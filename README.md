# hello-world

Before explaining CodeIgniter’s approach to data validation, let’s describe the ideal scenario:

A form is displayed.
You fill it in and submit it.
If you submitted something invalid, or perhaps missed a required item, the form is redisplayed containing your data along with an error message describing the problem.
This process continues until you have submitted a valid form.
On the receiving end, the script must:

Check for required data.
Verify that the data is of the correct type, and meets the correct criteria. For example, if a username is submitted it must be validated to contain only permitted characters. It must be of a minimum length, and not exceed a maximum length. The username can’t be someone else’s existing username, or perhaps even a reserved word. Etc.
Sanitize the data for security.
Pre-format the data if needed (Does the data need to be trimmed? HTML encoded? Etc.)
Prep the data for insertion in the database.