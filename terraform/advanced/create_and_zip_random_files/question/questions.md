Use the terraform files provided in this problem repo and implement a `main.tf` that does the following.

* Use the `filenames` variable provided in `vars.tfvars` to create a file for each filename.
* Use the `file_contents.tpl` file to populate the contents of each file with the template variables populated
    * `filename` should be the name of the current file
    * `random_data` should be a random string of length 16, and different for each file
* zip the resulting files in to a file named `random.zip`
* any config options not explicitly stated can be left as their defaults


Variable definitions, values, and provider config are provided and you will implement the data and resources necessary.

Please return the following as your answer
* main.tf
* random.zip
* terraform.tfstate
