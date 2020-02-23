# Manually installing the Open Data Hub 
This procedure describes how to install the Open Data Hub operator into your project namespace on OpenShift 3.11 
and is based on procedures


## Prerequisites
1.	Access to OpenShift using an account with **cluster-admin** privileges available. You will need the 
    **cluster-admin** privileges to create the **OpenDataHub** custom resource definition, and to apply the 
    **anyuid** security context constraint (SCC) for the Ceph container.
2.	A terminal shell with the OpenShift client command **oc** availabe.
3.	A copy of the files in this repository available in your terminal shell.
1.  A working knowledge of Kubernetes.
1.  A target cluster with access to the internet and the ability to pull from public container registries.

## Installing the Operator Lifecycle Manager (OLM)

The Operator Lifecycle Manager (OLM) is a tool to help manage the Operators running on your cluster.

If you are running OpenShift 3.11 determkne if the OLM is already installed. Note the OLM is installed in OpenShift version 4.x by default

1. Log onto OpenShift Cluster 
![image](./images/oc-cluster-catalog.png)

1. Determine if you already have OLM installed by accessing the **Cluster Console**
If you see Operator in list on left you can skip this section. 

![image](./images/oc-cluster-console-1.png)

1. If not run the following command to install the OLM:

```

$ curl -sL https://github.com/operator-framework/operator-lifecycle-manager/releases/download/0.11.0/install.sh | bash -s 0.11.0

```

1. Verify that OLM has een successfully installed into OpenShift Cluster by access Cluster Console again.

![image](./images/oc-cluster-console-2.png)

## References
1.	operator-lifecycle-manager, https://github.com/operator-framework/operator-lifecycle-manager , A management framework for extending Kubernetes with Operators
2.	Opendatahub-operator, https://gitlab.com/opendatahub/opendatahub-operator/-/tree/master
3.	Manually Install OpenData Hub, https://gitlab.com/opendatahub/opendatahub-operator/-/blob/master/docs/manual-installation.adoc




![image](./images/imageA.png)

![image](./images/imageB.png)

![image](./images/imageC.png)
![image](./images/imageD.png)

![image](./images/imageE.png)

![image](./images/imageF.png)