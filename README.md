# instabot-python-app
Creates a docker image with instabot and schedule inside

## build

    docker build -t csenf/instabot-python-app .
    
    docker image save --output "csenf_instabot-python-app_latest.tar"  csenf/instabot-python-app
    
## run

1. create a python script that uses instabot inside.
    
    inspiration can be found in [examples folder of instabot](https://github.com/instagrambot/instabot/tree/master/examples)

1. run docker in current directory


    docker run -it --rm --name instabot-python-app -v "$PWD":/usr/src/app csenf/instabot-python-app:latest python fancy_instagram_bot_script.py
    
## credits

- [instabot](https://github.com/instagrambot/instabot)