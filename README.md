# gcloud_commands

main gcloud and gsutil commands for GCP

# create a project GCP
> gcloud projects create my-project-bla-bla-bla

# list all disks in select project
> gcloud compute disks list

# list configurations
> glcoud config list

# list all projects
> gcloud projects list

# list all configurations
> gcloud config configurations list

# change project
> gcloud config set project project_id

# list all organizations
> gcloud organizations list

# list all emails for auth
> gcloud auth list

# list all components instaled
> gcloud components list

# Como compartilhar snapshots entre projetos
> gcloud compute disks snapshot disk-1 --project project-a --snapshot-names snapshot-1

> gcloud compute disks create disk-2  --project project-b --source-snapshot projects/project-a/global/snapshots/snapshot-1

> gcloud compute instances attach-disk instance-1 --project project-b --disk disk-2
