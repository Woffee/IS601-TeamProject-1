## Docker on AWS

What good is an application that can't be shared with friends, right? So in this section we are going to see how we can deploy our awesome application to the cloud so that we can share it with our friends! We're going to use AWS Elastic Beanstalk to get our application up and running in a few clicks. We'll also see how easy it is to make our application scalable and manageable with Beanstalk!

### Docker push

The first thing that we need to do before we deploy our app to AWS is to publish our image on a registry which can be accessed by AWS. There are many different Docker registries you can use (you can even host your own). For now, let's use Docker Hub to publish the image.

If this is the first time you are pushing an image, the client will ask you to login. Provide the same credentials that you used for logging into Docker Hub.

    $ docker login
    Login in with your Docker ID to push and pull images from Docker Hub. If you do not have a Docker ID, head over to https://hub.docker.com to create one.
    Username: yourusername
    Password:
    WARNING! Your password will be stored unencrypted in /Users/yourusername/.docker/config.json
    Configure a credential helper to remove this warning. See
    https://docs.docker.com/engine/reference/commandline/login/credential-store
    
    Login Succeeded
    
To publish, just type the below command remembering to replace the name of the image tag above with yours. It is important to have the format of yourusername/image_name so that the client knows where to publish.

    $ docker push yourusername/catnip
    
Once that is done, you can view your image on Docker Hub. For example, here's the web page for my image.

Note: One thing that I'd like to clarify before we go ahead is that it is not imperative to host your image on a public registry (or any registry) in order to deploy to AWS. In case you're writing code for the next million-dollar unicorn startup you can totally skip this step. The reason why we're pushing our images publicly is that it makes deployment super simple by skipping a few intermediate configuration steps.

Now that your image is online, anyone who has docker installed can play with your app by typing just a single command.

    $ docker run -p 8888:5000 yourusername/catnip

If you've pulled your hair out in setting up local dev environments / sharing application configuration in the past, you very well know how awesome this sounds. That's why Docker is so cool!

