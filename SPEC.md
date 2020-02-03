# data tree 

example
```yaml
resume:
  name:
    jp: じゅんぺい
    en: junpayment
  picture: https://junpayment.com/picture.png
  birth: 1985-01-30
  sex: male[female|none|and so on...]
  address:
    zip: 1111111
    address:
      jp: xxxxxxxx
      en: yyyyyyyy 
  contact:
    tel: 00000000000
    email: junpayment@mail.com
  snss:
    - type: github
      name: junpayment
    - type: twitter
      name: junpayment
  skills:
    - name: golang
      description: xxxxxxxxx
    - name: gcp
      description: xxxxxxxxx
  educational_background:
    school:
      jp: xxxxxxxx
      en: yyyyyyyy 
    faculty:
      jp: xxxxxxxx
      en: yyyyyyyy 
    terms:
      start: 2010-04-01
      end: 2013-03-31
  works:
    - company: somecompany
      title:
        jp: xxxxxxxx
        en: yyyyyyyy 
      what_i_do:
        jp: xxxxxxxx
        en: yyyyyyyy 
      terms:
        start: 2015-04-01
        end: 2016-03-31
      skills:
        - golang
        - gke
compnies:
  - id: somecompany
    name:
      jp: xxxxxxxx
      en: yyyyyyyy 
    url: https://somecompany.com
acl:
  target: resume.address
  permissions: company
```

# Supports ACL(readonly access control)
Control to whom distribute by acl.  

example
```yaml
acl:
  target: resume.address
  permissions: company
```

```yaml
acl:
  target: resume.name
  permissions: everyone
```

# String items can be supported multiple languages
example
```yaml
  name:
    jp: じゅんぺい
    en: junpayment
```

