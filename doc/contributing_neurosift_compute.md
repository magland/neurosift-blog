# Contributing Neurosift Compute

Many of the visualizations in Neurosift require precomputation of data on the DANDI Archive. This is handled using Dendro compute clients that continually listen for new jobs. If you would like to contribute your CPU cycles to this effort, following these steps:

Preqrequisites: A Linux or MacOS machine with Docker or Apptainer installed.

1. Ask the Neurosift team for permission to process jobs on the neurosift Dendro service. We will authorize your GitHub username to submit jobs.
2. Register a Dendro compute client on the neurosift channel (see below).
3. Configure the compute client to allocate resources to the Dendro service (see below).
4. Run the compute client to begin processing jobs (see below).

## Registering the Dendro compute client

By running a compute client on your computer, you are allowing Neurosift to send containerized jobs to your computer for execution.

Prerequisites: Python 3.7 or later as well as docker or apptainer.

First install dendro

```bash
pip install --upgrade dendro
```

Then create a new directory for your compute client

```bash
mkdir dendro_compute_client
cd dendro_compute_client
```

Register the compute client

```bash
dendro register-compute-client
```

When prompted for the service name, enter "neurosift".

When prompted for a name of the compute client, use a short name that identifies you or your computer.

Click the link to complete the configuration. You will be redirected to a page where you can log in using GitHub and authorize the compute client.

Finally, start the compute client.

```bash
CONTAINER_METHOD=apptainer dendro start-compute-client
```

You can either use docker or apptainer as the container method. If you use apptainer, you will need to have apptainer installed. If you use docker, you will need to have docker installed and running.

You should see a link to configure your compute client. Click the link and specify the resources you want to allocate to the compute client.

Finally stop the compute client (Ctrl+C) and restart it to apply the changes.