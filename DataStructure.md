# Data Structure

## example

var portals = {
    "Portal-Editor" : {
        portalID : "Portal-Editor"
        files : {
            "/docs/me/readme.txt" : {
                occupier : ["user1", "user2", "user3"],
                activeUser : ["user2"]
            },
            "/docs/me/readme.docx" : {
                occupier : ["user1", "user4"],
                activeUser : ["user1"]
            }
        },
        users : {
            "user1" : {
                userId : "user1",
                portalId : "Portal-Editor"
            },
            // ...
        }
    }
}