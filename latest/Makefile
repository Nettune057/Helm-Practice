runargs := $(word 3, $(MAKECMDGOALS))
nameargs := $(word 2, $(MAKECMDGOALS))


install:
	helm install ${nameargs} . -f ./env/${runargs}/values.${runargs}.yaml

upgrade:
	helm upgrade ${nameargs} . -f ./env/${runargs}/values.${runargs}.yaml
	
delete:
	helm delete ${nameargs} 