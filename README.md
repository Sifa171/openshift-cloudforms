# openshift-cloudforms

This template is related to a DockerImage created by Red Hat, which is in state tech preview. If you need more information, then take a look at this blog: http://cloudformsblog.redhat.com/2016/09/14/cloudforms-as-a-container/

# how to get it work

First of all you have to clone this repo and follow these few steps.

```
$ oc new-project cfme --display-name="Cloudforms Management Environment" 

$ oc create serviceaccount cfmesvcacc -n cfme

$ oadm policy add-scc-to-user privileged system:serviceaccount:cfme:cfmesvcacc 

$ oc create -f openshift-cloudforms-template.json
```

# my versions

1) OpenShift Origin 1.3

2) Cloudforms 4.1 

# outcome

![OCSP Project Overview](https://github.com/Sifa91/openshift-cloudforms/blob/master/doc/oscp_overview.png)

![CFME Login](https://github.com/Sifa91/openshift-cloudforms/blob/master/doc/login.png)

![CFME Overview](https://github.com/Sifa91/openshift-cloudforms/blob/master/doc/cfme_overview.png)
