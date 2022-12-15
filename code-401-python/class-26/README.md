
## [DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)

- permission checks are done before any of the main code starts running
- An exeption will be raised if permission is not given and a 400 error will be recived
- classes control permissions
- AllowAny will give access to anyone
- permissions can be set in settings.py or views
- There are API reverence classes that will allow you to set different permissions
- Third party packages are also available
- can create custom permissions

### API Reference

- IsAuthenticated
- AllowAny
- IsAuthenticatedOrReadOnly
- IsAdminUser
- DjangoModelPermissions
- DjangoModelPermissionsOrAnonReadOnly
- Custom permissions
- DjangoObjectPermissions

### Third party packages

- DRF - Access Policy
- Composed Permissions
- DRY Rest Permissions
- REST Condition
- Django REST Framework API Key
- Django Rest Framework Roles
- Django Rest Framework Role Filters
- Django Rest Framework PSQ


## Bookmark

- [Classy Django REST](http://www.cdrf.co/)
- [DRF Generic Views](https://www.django-rest-framework.org/api-guide/generic-views/)