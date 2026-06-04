# rules_img

This example shows how `rules_buildx` can be used with `rules_img`.

A Dockerfile is used to install `git` on Debian.
The default entrypoint outputs `git --version`.
The image is exported as an OCI directory and then imported to `rules_img`.

Add the image to your local registry:

```bash
bazel run //:image_load
```

Run the image:

```bash
docker run --rm bazel/rules_img_buildx_demo:latest
```
