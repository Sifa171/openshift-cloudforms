# openshift-cloudforms

# How to get it work

First of all you have to clone this repo and follow these few steps.

1) $ oc new-project cfme --display-name="Cloudforms Management Environment" 

2) $ oc create serviceaccount cfmesvcacc -n cfme

3) $ oadm policy add-scc-to-user privileged system:serviceaccount:cfme:cfmesvcacc 

4) 
