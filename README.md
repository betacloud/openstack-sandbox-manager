# openstack-sandbox

## Usage

* Create `clouds.yml` on basis of `clouds.yml.sample`
* Create `secure.yml` on basis of `secure.yml.sample`

Show resources that are older than `THRESHOLD` days:

```
$ tox -e list -- --cloud sandbox --projectname sandbox --domainid DOMAIN_ID --threshold THRESHOLD
```

Send a notification to an owner whose resource is older than `THRESHOLD` days:

```
$ tox -e list -- --cloud sandbox --projectname sandbox --domainid DOMAIN_ID --threshold THRESHOLD --mailgunkey MAILGUN_API_KEY
```
