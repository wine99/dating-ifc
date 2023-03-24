dating-server:
	$(TROUPE)/bin/troupec dating-server.trp -o ./out/dating-server.js
	node $(TROUPE)/rt/built/troupe.js -f=./out/dating-server.js --id=../ids/id-server.json --trustmap=../trustmaps/GoT.json --aliases=aliases.json

dating-client:
	$(TROUPE)/bin/troupec dating-client.trp -o ./out/dating-client.js
	node $(TROUPE)/rt/built/troupe.js -f=./out/dating-client.js --trustmap=../trustmaps/client.json

# dating-goodman:
# 	$(TROUPE)/bin/troupec dating-goodman.trp -o ./out/dating-goodman.js
# 	node $(TROUPE)/rt/built/troupe.js -f=./out/dating-goodman.js --id=../ids/id-goodman.json --trustmap=../trustmaps/client-goodman.json
dating-goodman:
	$(TROUPE)/bin/troupec dating-goodman.trp -o ./out/dating-goodman.js
	node $(TROUPE)/rt/built/troupe.js -f=./out/dating-goodman.js --id=../ids/id-goodman.json