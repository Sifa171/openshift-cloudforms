# openshift-cloudforms

This template is related to a DockerImage created by Red Hat, which is in state tech preview. If you need more information, then take a look at this blog: http://cloudformsblog.redhat.com/2016/09/14/cloudforms-as-a-container/

# how to get it work

First of all you have to clone this repo and follow these few steps.

1) $ oc new-project cfme --display-name="Cloudforms Management Environment" 

2) $ oc create serviceaccount cfmesvcacc -n cfme

3) $ oadm policy add-scc-to-user privileged system:serviceaccount:cfme:cfmesvcacc 

4) $ oc create -f openshift-cloudforms-template.json


# my versions

1) OpenShift Origin 1.3

2) Cloudforms 4.1 

# outcome

![alt tag](http://url/to/img.png)
