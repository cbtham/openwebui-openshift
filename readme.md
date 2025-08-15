# Deploy OpenWebUI on OpenShift
This is use for demo purposes. If you want to reference this as a deployment for prod, please go through the yaml to enable authentication and configure necessary parameters.

### This will create
1. A persistent volume
1. A persistent volume claim
1. OpenWebUI application
1. A service
1. A route

## Deployment
1. Git clone this repository
1. Create a new project or go to an exisiting one.
    ```shell
    oc new-project openwebui
    oc project openwebui
    ```
1. Deploy by running
    ```shell
    oc create -f openwebui-openshift/openwebui.yaml
    ```

## Connecting to a private endpoint

Go to settings, create a connection and put in the private AI endpoint. After that refresh your browser and you will see the models showing.