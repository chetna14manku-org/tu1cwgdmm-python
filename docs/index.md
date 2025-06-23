# Trusted Application Pipeline Software Template

This application, **tu1cwgdmm-python**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/chetna14manku-org/tu1cwgdmm-python ](https://github.com/chetna14manku-org/tu1cwgdmm-python ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/chetna14manku-org/tu1cwgdmm-python-gitops ](https://github.com/chetna14manku-org/tu1cwgdmm-python-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |
| **tssc-app-ci** | The namespace used for CI workloads |
| **tssc-app-development** | The default application during development. Every build will be deployed to this namespace for testing. |
| **tssc-app-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/chetna14manku-org/tu1cwgdmm-python-gitops ) in the components/tu1cwgdmm-python/overlays/stage directory |
| **tssc-app-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/chetna14manku-org/tu1cwgdmm-python-gitops ) in the components/tu1cwgdmm-python/overlays/prod directory |