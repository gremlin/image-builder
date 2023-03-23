# Image Builder for Cluster API

The Image Builder can be used to build images intended for use with Kubernetes [CAPI](https://cluster-api.sigs.k8s.io/) providers. Each provider has its own format of images that it can work with. For example, AWS instances use AMIs, and vSphere uses OVAs.

For detailed documentation, see https://image-builder.sigs.k8s.io/capi/capi.html.

### For Gremlins

When building a new image, be sure to set the AWS_PROFILE appropriately.

To build a new image, run

```
PACKER_VAR_FILES=gremlin-shift.json make build-ami-ubuntu-2204
```
