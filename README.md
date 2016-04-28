# edc-templates


The templates override the admin templates to add

- add instructions at the top of each form
- add footer to each page with a disclaimer, protocol version number and software version number (from git)
- add next_url querystring parameter to override redirect after an ModelAdmin form is saved 
- save next button on Add forms that redirects after save to the next required form

In order for the templates to be used project wide, put `edc_templates` at the top of `INSTALLED_APPS`:

	INSTALLED_APPS = (
	    'edc_templates',
	    'django.contrib.admin',
	    'django.contrib.auth',
	    'django.contrib.contenttypes',
	    'django.contrib.sessions',
	    'django.contrib.messages',
	    'django.contrib.staticfiles',
	    'edc_base',
		...
    )
