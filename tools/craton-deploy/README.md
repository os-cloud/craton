# Deploying Craton

``` shell
cp etc/openstack_deploy/conf.d/* /etc/openstack_deploy/conf.d/
cp etc/openstack_deploy/env.d/* /etc/openstack_deploy/env.d/
```

``` shell
echo 'craton_db_password: secrete' | tee -a /etc/openstack_deploy/user_secrets.yml
echo 'craton_admin_password: SuperSecrete' | tee -a /etc/openstack_deploy/user_secrets.yml
```

``` shell
openstack-ansible deploy-creaton.yml
```
