<!--[metadata]>
+++
title = "system prune"
description = "Remove unused data"
keywords = [system, prune, delete, remove]
[menu.main]
parent = "smn_cli"
+++
<![end-metadata]-->

# system prune

```markdown
Usage:	docker system prune COMMAND

Delete unused data

Options:
  -a, --all     Remove all unused images not just dangling ones
  -f, --force   Do not prompt for confirmation
      --help    Print usage
```

Remove all unused containers, volumes and images (both dangling and unreferenced).

Example output:

```bash
$ docker system prune -a
WARNING! This will remove:
	- all stopped containers
	- all volumes not used by at least one container
	- all images without at least one container associated to them
Are you sure you want to continue? [y/N] y
Deleted Containers:0998aa37185a1a7036b0e12cf1ac1b6442dcfa30a5c9650a42ed5010046f195b
73958bfb884fa81fa4cc6baf61055667e940ea2357b4036acbbe25a60f442a4d

Deleted Volumes:
named-vol

Deleted Images:
untagged: my-curl:latest
deleted: sha256:7d88582121f2a29031d92017754d62a0d1a215c97e8f0106c586546e7404447d
deleted: sha256:dd14a93d83593d4024152f85d7c63f76aaa4e73e228377ba1d130ef5149f4d8b
untagged: alpine:3.3
deleted: sha256:695f3d04125db3266d4ab7bbb3c6b23aa4293923e762aa2562c54f49a28f009f
untagged: alpine:latest
deleted: sha256:ee4603260daafe1a8c2f3b78fd760922918ab2441cbb2853ed5c439e59c52f96
deleted: sha256:9007f5987db353ec398a223bc5a135c5a9601798ba20a1abba537ea2f8ac765f
deleted: sha256:71fa90c8f04769c9721459d5aa0936db640b92c8c91c9b589b54abd412d120ab
deleted: sha256:bb1c3357b3c30ece26e6604aea7d2ec0ace4166ff34c3616701279c22444c0f3
untagged: my-jq:latest
deleted: sha256:6e66d724542af9bc4c4abf4a909791d7260b6d0110d8e220708b09e4ee1322e1
deleted: sha256:07b3fa89d4b17009eb3988dfc592c7d30ab3ba52d2007832dffcf6d40e3eda7f
deleted: sha256:3a88a5c81eb5c283e72db2dbc6d65cbfd8e80b6c89bb6e714cfaaa0eed99c548

Total reclaimed space: 13.5 MB
```

## Related information

* [volume create](volume_create.md)
* [volume ls](volume_ls.md)
* [volume inspect](volume_inspect.md)
* [volume rm](volume_rm.md)
* [Understand Data Volumes](../../tutorials/dockervolumes.md)
* [system df](system_df.md)
* [container prune](container_prune.md)
* [image prune](image_prune.md)
* [system prune](system_prune.md)
