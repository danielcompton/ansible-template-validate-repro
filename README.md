# ansible-template-validate-repro 

Example project to reproduce [ansible/ansible#41377](https://github.com/ansible/ansible/issues/41377#issuecomment-396580050).

## Running

First, set your preferred GCP project ID in repro-image.json under `"project_id"`, e.g. `my-app`. If you haven't already, you may need to install `gcloud` and authenticate it with it. See the [Packer docs](https://www.packer.io/docs/builders/googlecompute.html) for more.

Then run:

```console
$ packer build repro-image.json
```