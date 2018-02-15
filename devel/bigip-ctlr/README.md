# k8s-bigip-ctlr

The F5 BIG-IP Controller for Kubernetes makes F5 BIG-IP Local Traffic Manager services available to applications running in Kubernetes.

## TL;DR;

Assuming you have added the apptio repo

```bash
$ helm install bigip-ctlr
```

## Configuration

|         Parameter                   |             Description                    |                         Default                          |
|----------------------------         |-------------------------------------       |----------------------------------------------------------|
| `bigip.username`                    | Username to connect to F5                  | `empty` (required)                                       |
| `bigip.password`                    | Password to connect to F5                  | `empty` (required)                                       |
| `bigip.url`                         | URL to use to connect to F5                | `empty` (required)                                       |
| `bigip.paritition`                  | F5 partition to manage with controller     | `empty` (required)                                       |
| `bigip.defaultip`                   | Default IP for the Virtual Servers         | `nil`                                                    |
| `bigip.dnsserver`                   | DNS Server to use to lookup ingresses      | `nil`                                                    |

