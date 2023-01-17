# Test to pass environemnts 

1- Export the environments you want:
export TMPDIR="path/to/something"
export USER="My User"

2- Execute the comand
echo CI_DIR=$TMPDIR >> environment-properties.env && echo USER=$USER >> environment-properties.env && kustomize build . && echo "" > environment-properties.env