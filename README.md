# `ncp-flat-kubeconfig`: Flat kubeconfig for NKS

[![version](https://img.shields.io/badge/version-0.2-yellow.svg)](https://semver.org)
![Proudly written in Bash](https://img.shields.io/badge/written%20in-bash-ff69b4.svg)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## **`ncp-flat-kubeconfig`** DEMO 
![ncp-flat-kubeconfig-demo GIF](img/ncp-flat-kubeconfig-demo.gif)

-----

## Prerequisite
Yaml Parser(yq)

## Environment
Support only NKS(Naver Kubernetes Serivce)

## Purpose 
NKS's kubeconfig name is duplicated. 
And it doesn't support to flat kubeconfig function yet. 
Thus use to flat and rename the kubeconfig. 

## Usage
kubeconfig.yaml is hard coded due to it fixed 
If it needs, I will change it. 
```bash 
$ ncp-flat-kubeconfig 
successfully flatting NKS's kubeconfig
```

-----

## Check

```bash
$ kubectl config get-contexts
CURRENT   | NAME       | CLUSTER     | AUTHINFO         | NAMESPACE
----      | ----       | ----        | ----             |  ----
*         | nks        | kubernetes  | kubernetes-admin |
          | nks-0346   | nks-KR-0346 | nks-user         | 
```

-----

## Installation

### One time runner 
`kubeconfig.yaml` must be in a same folder
```bash 
curl https://raw.githubusercontent.com/sysnet4admin/ncp-flat-kubeconfig/main/ncp-flat-kubeconfig | bash
```

### Installation (macOS and Linux)

```bash
curl https://raw.githubusercontent.com/sysnet4admin/ncp-flat-kubeconfig/main/install | bash
```

