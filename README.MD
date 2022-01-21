# Create this Static Site

---
**NOTE**

This is a work in progress

---

## Object Storage Steps

1. Create an access key and secret key.
1. Create a new Object Storage bucket.
1. Install s3cmd command-line tool and configure it with your access keys.
1. Configure your bucket to host a website.
    s3cmd ws-create --ws-index=index.html --ws-error=404.html s3://my-bucket -c .s3cfg_myconfig

## CI/CD Steps

1. Create environment variables to store your Object Storage bucket credentials.
1. Create .github/workflows/workflow.yml directories and file.
1. Add the configurations from https://github.com/marketplace/actions/s3-sync to your workflow.yml file.