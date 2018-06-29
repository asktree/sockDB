# sockDB
sockDB is a personal database system designed to maximize the portability of your information between softwares. 

Items in sockDB are represented arbitrarily linked documents. Since support for arbitrary relationships between information requires (often untenable) design tradeoffs in software, sockDB can label and maintain non-arbitrary structural invariants (such as trees) in item subgraphs. This allows structurally constrained information to remain maximally portable between softwares with different structural requirements. 

## sockdb v0
* db items invariant
  * out = array of links
  * name = string
  * type = text | localpath | url
  * content = something of the given type
  * meta = {created = datetime; edited = datetime;}
  * invariants = array of structual invariants
* db link invariant
  * target = db item
  * source = db item
  * invariants = array of structual invariants
  * meta = {created = datetime}
  * [.value = a number] (optional)
* db invariant... invariant
