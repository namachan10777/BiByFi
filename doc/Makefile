SATYSFI_OPTS+=-b
ifdef SATYSFI_RUNTIME
	SATYSFI_OPTS+=-C "$(SATYSFI_RUNTIME)"
endif

doc.pdf: doc.saty local.satyh
	satysfi $(SATYSFI_OPTS) $< -o $@
