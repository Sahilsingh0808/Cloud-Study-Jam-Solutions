# GSP094
[![](https://github.com/CodingWithHardik/CodingWithHardik/blob/main/img/subscribe_button.png)](https://www.youtube.com/@CloudHustlers)
## Run in cloudshell
```cmd
sudo apt-get install -y virtualenv
python3 -m venv venv
source venv/bin/activate
pip install --upgrade google-cloud-pubsub
git clone https://github.com/googleapis/python-pubsub.git
cd python-pubsub/samples/snippets
python publisher.py $GOOGLE_CLOUD_PROJECT create MyTopic
python subscriber.py $GOOGLE_CLOUD_PROJECT create MyTopic MySub
```
