# Access to ui altair
https://localhost:7068/ui/altair

query {
  products {
    id,
    name,
    quantity
  }
}

query {
  products1: products {
    id,
    name,
  },
  products2: products {
    quantity
  },
  product(id: 2) {
    name,
    quantity
  }
}

====================
query ($id: Int!) {
  product(id: $id){
    name
  }
}

Variables: {"id": 1}
=====================
