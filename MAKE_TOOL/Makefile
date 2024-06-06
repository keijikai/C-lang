product: intermediate1 intermediate2
	@echo "building product"
	cat intermediate1 intermediate2 > product

intermediate1: source1
	@echo "building intermediate1"
	echo "this line is added" | cat source1 - > intermediate1

intermediate2: source2
	@echo "building intermediate2"
	echo "this line is added" | cat source2 - > intermediate2

