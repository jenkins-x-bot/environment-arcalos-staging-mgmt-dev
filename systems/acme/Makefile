init:
	helm init --client-only

build: clean init
	jx step helm build --boot --verbose=true
	helm lint .

clean: 
	rm -rf charts
	rm -rf requirements.lock
