# fungcorps

Make sure server is on before doing the below.

Check if someone else is on the server:
```
>> who
```

Check current resource usage:
```
>> htop
```

Check GPU usage (with 1 sec update rate):
```
>> nvidia-smi -l 1
```

## 1.0 Instructions to Access Machine Learning Server ##
```
>> ssh *username*@*server.net* (ask barn for your login and pw)
```  
## 2.0 Instructions for fast.ai ##

Clone the [fastai repo](https://github.com/fastai/fastai):
```
>> git clone https://github.com/fastai/fastai
```

Activate the fastai anaconda environment:
```
>> cd ~/directory to fastai local repo/fastai/
>> source activate fastai 
``` 
Run the jupyter notebook server for DL1:

First, find the local ipv4 address for the machine:
```
>> ifconfig
```
Then activate the notebook server at a convenient port:
```
>> cd ~/directory to fastai local repo/fast_ai/fastai/courses/dl1
>> jupyter notebook --ip *server local address* --port *4 digit port*
```
The terminal should output some instruction like this:
```
Copy/paste this URL into your browser when you connect for the first time,
    to login with a token:
     
```
Paste the URL into a browser and things should work.
