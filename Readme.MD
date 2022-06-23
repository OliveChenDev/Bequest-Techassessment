1 mongodb install & run
2 yarn
3 yarn start
4 query

read all
# {
#   books {
#     _id
#     title
#     author
#   }
# }

create
# mutation {
#   addBook(
#     isbn: "12345678",
#     title: "Whatever this Book Title",
#     author: "Mr. Bean",
#     description: "The short explanation of this Book",
#     publisher: "Djamware Press",
#     published_year: 2019
#   ) {
#     updated_date
#   }
# }

read one
# {
#   book(id: "62b35725098f0438f4ff662e") {
#     _id
#     isbn
#     title
#     author
#     description
#     published_year
#     publisher
#     updated_date
#   }
# }

update
# mutation {
#   updateBook(
#     id: "62b35725098f0438f4ff662e",
#     isbn: "12345678221",
#     title: "The Learning Curve of GraphQL",
#     author: "Didin J.",
#     description: "The short explanation of this Book",
#     publisher: "Djamware Press",
#     published_year: 2019
#   ) {
#     _id,
#     updated_date
#   }
# }

remove
# mutation {
#   removeBook(id: "62b35725098f0438f4ff662e") {
#     _id
#   }
# }
