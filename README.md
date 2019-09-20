# route-watcher - Andible Based

currently watching for only newely created objects, not for existing objects that been modified 

you can watch any object you want. just replace api-version and kind. you don't need to create CRD as the api already exists.

```
operator-sdk new route-watcher --api-version=route.openshift.io/v1 --kind=Route --type=ansible
```

# apache-operator - ansible based

this operator can listen events and trigger the plabook. you can write your own login inside the playbook

documentation is here https://github.com/operator-framework/operator-sdk/blob/master/doc/ansible/user-guide.md


to test locally

when testing locally replace role to absolute path - https://github.com/rajmechi/route-watcher/blob/master/watches.yaml#L5

operator-sdk up local





