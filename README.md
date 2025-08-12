<p align="center">
  <img src="https://i.postimg.cc/zGnjJnxg/Screenshot-2025-08-12-190543.png" 
       alt="Screenshot" 
       width="400" 
       height="250" />
</p>


<p align="center">
  <b><i>3HUE Security Agent</b> is the Open Cloud Security platform trusted by thousands to automate security and compliance in any cloud environment. With hundreds of ready-to-use checks and compliance frameworks, delivers real-time, customizable monitoring and seamless integrations, making cloud security simple, scalable, and cost-effective for organizations of any size.
</p>
<p align="center">

</p>
<hr>
<p align="center">
  <a href="https://goto.prowler.com/slack"><img alt="Slack Shield" src="https://img.shields.io/badge/slack-prowler-brightgreen.svg?logo=slack"></a>
  <a href="https://pypi.org/project/prowler/"><img alt="Python Version" src="https://img.shields.io/pypi/v/prowler.svg"></a>
  <a href="https://pypi.python.org/pypi/prowler/"><img alt="Python Version" src="https://img.shields.io/pypi/pyversions/prowler.svg"></a>
  <a href="https://hub.docker.com/r/toniblyx/prowler"><img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/toniblyx/prowler"></a>
  <a href="https://hub.docker.com/r/toniblyx/prowler"><img alt="Docker" src="https://img.shields.io/docker/cloud/build/toniblyx/prowler"></a>
  <a href="https://hub.docker.com/r/toniblyx/prowler"><img alt="Docker" src="https://img.shields.io/docker/image-size/toniblyx/prowler"></a>
  <a href="https://gallery.ecr.aws/prowler-cloud/prowler"><img width="120" height=19" alt="AWS ECR Gallery" src="https://user-images.githubusercontent.com/3985464/151531396-b6535a68-c907-44eb-95a1-a09508178616.png"></a>
  <a href="https://codecov.io/gh/prowler-cloud/prowler"><img src="https://codecov.io/gh/prowler-cloud/prowler/graph/badge.svg?token=OflBGsdpDl"/></a>
</p>
<p align="center">
  <a href="https://github.com/prowler-cloud/prowler"><img alt="Repo size" src="https://img.shields.io/github/repo-size/prowler-cloud/prowler"></a>
  <a href="https://github.com/prowler-cloud/prowler/issues"><img alt="Issues" src="https://img.shields.io/github/issues/prowler-cloud/prowler"></a>
  <a href="https://github.com/prowler-cloud/prowler/releases"><img alt="Version" src="https://img.shields.io/github/v/release/prowler-cloud/prowler"></a>
  <a href="https://github.com/prowler-cloud/prowler/releases"><img alt="Version" src="https://img.shields.io/github/release-date/prowler-cloud/prowler"></a>
  <a href="https://github.com/prowler-cloud/prowler"><img alt="Contributors" src="https://img.shields.io/github/contributors-anon/prowler-cloud/prowler"></a>
  <a href="https://github.com/prowler-cloud/prowler"><img alt="License" src="https://img.shields.io/github/license/prowler-cloud/prowler"></a>

</p>
<hr>

# Description

**3HUE Security Agent** is an open-source security tool designed to assess and enforce security best practices across AWS, Azure, Google Cloud, and Kubernetes. It supports tasks such as security audits, incident response, continuous monitoring, system hardening, forensic readiness, and remediation processes.

3HUE Security Agent includes hundreds of built-in controls to ensure compliance with standards and frameworks, including:

- **Industry Standards:** CIS, NIST 800, NIST CSF, and CISA
- **Regulatory Compliance and Governance:** RBI, FedRAMP, and PCI-DSS
- **Frameworks for Sensitive Data and Privacy:** GDPR, HIPAA, and FFIEC
- **Frameworks for Organizational Governance and Quality Control:** SOC2 and GXP
- **AWS-Specific Frameworks:** AWS Foundational Technical Review (FTR) and AWS Well-Architected Framework (Security Pillar)
- **National Security Standards:** ENS (Spanish National Security Scheme)
- **Custom Security Frameworks:** Tailored to your needs

## 3HUE Security Agent App

3HUE Security Agent App is a web-based application that simplifies running across your cloud provider accounts. It provides a user-friendly interface to visualize the results and streamline your security assessments.


## 3HUE Security Agent Dashboard

```console
3HUE-Security Agent dashboard
```
<p align="center">
  <img src="https://i.postimg.cc/FFjsQ7xd/Screenshot-2025-08-12-190400.png" alt="Screenshot">
</p>

# 3HUE Security Agent at a Glance

| Provider | Checks | Services | Compliance Frameworks | Categories|
|---|---|---|---|---|
| AWS | 567 | 82 | 36 | 10 |
| GCP | 79 | 13 | 10 | 3 |
| Azure | 142 | 18 | 11 | 3 |
| Kubernetes | 83 | 7 | 5 | 7 |
| GitHub | 16 | 2 | 1 | 0 |
| M365 | 69 | 7 | 3 | 2 |
| NHN (Unofficial) | 6 | 2 | 1 | 0 |

# 💻 Installation

## 3HUE Security Agent App

3HUE Security Agent App offers flexible installation methods tailored to various environments:

### Docker Compose

**Requirements**

* `Docker Compose` installed: https://docs.docker.com/compose/install/.

**Commands**

``` console
curl -LO https://github.com/OCTO-Hurricane/3HUE-Security-Scanner.git
docker compose up -d
```

> Containers are built for `linux/amd64`.

### Configuring Your Workstation for 3HUE Security Agent App

If your workstation's architecture is incompatible, you can resolve this by:

- **Setting the environment variable**: `DOCKER_DEFAULT_PLATFORM=linux/amd64`
- **Using the following flag in your Docker command**: `--platform linux/amd64`

> Once configured, access the 3HUE Security Agent App at http://localhost:3000. Sign up using your email and password to get started.

### Common Issues with Docker Pull Installation

> [!Note]
  If you want to use AWS role assumption (e.g., with the "Connect assuming IAM Role" option), you may need to mount your local `.aws` directory into the container as a volume. There are several ways to configure credentials for Docker containers. See the [Troubleshooting](./docs/troubleshooting.md) section for more details and examples.

You can find more information in the [Troubleshooting](./docs/troubleshooting.md) section.


### From GitHub

**Requirements**

* `git` installed.
* `poetry` v2 installed: [poetry installation](https://python-poetry.org/docs/#installation).
* `npm` installed: [npm installation](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm).
* `Docker Compose` installed: https://docs.docker.com/compose/install/.

**Commands to run the API**

``` console
git clone https://github.com/OCTO-Hurricane/3HUE-Security-Scanner.git
cd 3HUE-Security-Scanner/api
poetry install
eval $(poetry env activate)
set -a
source .env
docker compose up postgres valkey -d
cd src/backend
python manage.py migrate --database admin
gunicorn -c config/guniconf.py config.wsgi:application
```
> [!IMPORTANT]
> As of Poetry v2.0.0, the `poetry shell` command has been deprecated. Use `poetry env activate` instead for environment activation.
>
> If your Poetry version is below v2.0.0, continue using `poetry shell` to activate your environment.
> For further guidance, refer to the Poetry Environment Activation Guide https://python-poetry.org/docs/managing-environments/#activating-the-environment.

> After completing the setup, access the API documentation at http://localhost:8080/api/v1/docs.

**Commands to run the API Worker**

``` console
git clone https://github.com/OCTO-Hurricane/3HUE-Security-Scanner.git
cd 3HUE-Security-Scanner/api
poetry install
eval $(poetry env activate)
set -a
source .env
cd src/backend
python -m celery -A config.celery worker -l info -E
```

**Commands to run the API Scheduler**

``` console
git clone https://github.com/OCTO-Hurricane/3HUE-Security-Scanner.git
cd 3HUE-Security-Scanner/api
poetry install
eval $(poetry env activate)
set -a
source .env
cd src/backend
python -m celery -A config.celery beat -l info --scheduler django_celery_beat.schedulers:DatabaseScheduler
```

**Commands to run the UI**

``` console
git clone https://github.com/OCTO-Hurricane/3HUE-Security-Scanner.git
cd 3HUE-Security-Scanner/ui
npm install
npm run build
npm start
```

> Once configured, access the 3HUE Security Agent App at http://localhost:3000. Sign up using your email and password to get started.

### Containers

**Available Versions of 3HUE Security Agent CLI**

The following versions of 3HUE Security Agent CLI are available, depending on your requirements:

- `latest`: Synchronizes with the `master` branch.

# ✏️ High level architecture

## 3HUE Security Agent App
**3HUE Security Agent App** is composed of three key components:

- **UI**: A web-based interface, built with Next.js, providing a user-friendly experience for executing scans and visualizing results.
- **API**: A backend service, developed with Django REST Framework, responsible for running scans and storing the generated results.
- **SDK**: A Python SDK designed to extend the functionality of the 3HUE Security Agent CLI for advanced capabilities.

## 3HUE Security Agent CLI

**Running 3HUE Security Agent **

3HUE Security Agent can be executed across various environments, offering flexibility to meet your needs. It can be run from:

- Your own workstation

- A Kubernetes Job

- Google Compute Engine

- Azure Virtual Machines (VMs)

- Amazon EC2 instances

- AWS Fargate or other container platforms

- CloudShell

And many more environments.

![Architecture](docs/img/architecture.png)

# 📃 License

**3HUE Security Agent License Information**

3HUE Security Agent is licensed under the Apache License 2.0.
