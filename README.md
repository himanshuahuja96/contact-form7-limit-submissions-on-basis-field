# contact-form7-limit-submissions-on-basis-field
Limit Submission of Contact Form 7 basis of IP 

How it works?
We add the user ip with each subission and after that before each submission we check whether the user can submit or not on basis of setting done in the configuration area for each contact form.

Dependency:
You need to install this plugin https://wordpress.org/plugins/contact-form-7-dynamic-text-extension/ to attach the userip to dynamic field shortcode which we will be installing and https://wordpress.org/plugins/contact-form-cfdb7/ is used for stroring and then quering the data to check whether the user is eligible to submit another input or not.

And add these shortcodes in the each contact form you want user to submit limited responses (both):
[dynamichidden client_ip "get_client_ip"]
[dynamichidden submittedat "get_submitted_at"]
