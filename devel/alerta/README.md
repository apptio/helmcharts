# Alerta

The alerta monitoring system is a tool used to consolidate and de-duplicate alerts from multiple sources for quick ‘at-a-glance’ visualisation. With just one system you can monitor alerts from many other monitoring tools on a single screen.

## TL;DR;

Assuming you have added the apptio repo

```bash
$ helm install --dep-up devel/stable
```

## Configuration

Alerta requires mongodb. See the [mongodb chart](https://github.com/kubernetes/charts/blob/master/stable/mongodb/README.md) for more details on the parameters to set there.

|         Parameter                   |             Description                    |                         Default                          |
|----------------------------         |-------------------------------------       |----------------------------------------------------------|
| `alertaAdminUsers`                  | A list of admin user emails (csv)          | `empty`                                                  |
| `alertaAdminPassword`               | Admin pass for all admins                  | `random alhpanumeric string (10)`                        |
| `alertaPlugins`                     | Plugins to enable                          |                                                          |
| `alertaInstallPlugins`              | Plugins to install                         |                                                          |
