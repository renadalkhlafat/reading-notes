# Django REST framework - Permissions
Permissions are used to grant or deny access for different classes of users to different parts of the API.


## Object level permissions
REST framework permissions also support object-level permissioning. Object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.

## How permissions are determined
Permissions in REST framework are always defined as a list of permission classes.

Before running the main body of the view each permission in the list is checked. If any permission check fails an exceptions.PermissionDenied or exceptions.NotAuthenticated exception will be raised, and the main body of the view will not run.

## Setting the permission policy
The default permission policy may be set globally, using the `DEFAULT_PERMISSION_CLASSES `setting.

**Example**

```python
REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.IsAuthenticated',
    ]
}
```
