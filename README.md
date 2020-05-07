# consul-demo

Repo in support of the following blog post: https://blog.baeke.info/2020/05/05/getting-started-with-consul-on-kubernetes/

Accompanying video: https://youtu.be/B5pWtJDapG4

The deployment manifest uses an image on Docker hub from the code folder in this repo. The container won't work without following the steps in the blog post or video.

The container needs a Consul deployment with Consul agents exposing their static port 8500 on the Kubernetes hosts. You also need to add a key/value pair: key=REDISPATTERN, value=*

You can deploy Kubernetes, Consul but also Flux using https://github.com/gbaeke/pulumi-samples/tree/master/aks-consul
