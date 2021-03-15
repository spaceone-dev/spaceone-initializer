# spaceone-initializer

SpaceONE initializer

# Root Domain

Root domain is a system domain for over-all user-domain.

* providing pluin service
* providing market-place service

## create vaules.yaml

Get market-place Token from spaceone administrator

~~~
enabled: true
image:
    name: spaceone/spacectl
    version: 1.6.2

domain: root
main:
  var:
    domain_owner:
      id: admin
      password: AdministratoR1
    marketplace_token: ____PUT_MARKET_PLACE_TOKEN_HERE_____________
~~~

helm install root-domain -f values.yaml spaceone/spaceone-initializer

# User Domain
