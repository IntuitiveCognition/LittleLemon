https://github.com/IntuitiveCognition/LittleLemon/tree/main




http://localhost:8000/docs/    # this address provides documentation for all API endpoints for the project.

This is created by adding the below code to the project urls.py

from rest_framework.documentation import include_docs_urls

urlpatterns = [
    ...
    path('docs/', include_docs_urls(title='Your Project API')),
]

adding this to your setting.py file
REST_FRAMEWORK = {
    
    'DEFAULT_SCHEMA_CLASS': 'rest_framework.schemas.coreapi.AutoSchema',

}

installing coreapi with pip or pipenv

