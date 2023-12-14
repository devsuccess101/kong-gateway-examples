.PHONY: kong
kong:
	helm -n kong-ingress upgrade \
		kong kong/ingress \
		--install \
		--create-namespace \
		--values ./ingress.values.yaml

	# For Kong Manager access
	# kubectl port-forward kong-gateway-77f57d75f8-4dcvr 8001:8001 8002:8002
	# http://localhost:8002
