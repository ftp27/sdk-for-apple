import Appwrite

let client = Client()
    .setEndpoint("https://[HOSTNAME_OR_IP]/v1") // Your API Endpoint
    .setProject("5df5acd0d48c2") // Your project ID

let account = Account(client)

let user = try await account.updatePhone(
    phone: "+12065550100",
    password: "password"
)

