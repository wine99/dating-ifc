MKID=node $(TROUPE)/rt/built/p2p/mkid.js
MKALIASES=node $(TROUPE)/rt/built/p2p/mkaliases.js
START=$(TROUPE)/bin/network.sh

zero.listener:
	$(START) zero.trp --id=ids/pingpong-listener.json --rspawn=true --aliases=aliases.json --debug --debugp2p

pingpong.dialer:
	$(START) p2ppingpong.trp --id=ids/pingpong-dialer.json --aliases=aliases.json  # --debug --debugp2p

create-network-identifiers:
	mkdir -p ids 
	$(MKID) --outfile=ids/pingpong-listener.json
	$(MKID) --outfile=ids/pingpong-dialer.json
	$(MKALIASES) --include ids/pingpong-listener.json --include ids/pingpong-dialer.json --outfile aliases.json
