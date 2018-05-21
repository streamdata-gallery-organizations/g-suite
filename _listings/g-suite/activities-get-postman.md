{
  "info": {
    "name": "G Suite Activity",
    "_postman_id": "8299e2dc-ca9c-4036-87a3-ee3302b1f5e7",
    "description": "Provides a historical view of activity.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "activities",
      "item": [
        {
          "id": "c59563a9-0094-4a1f-a989-c56eee59d6c3",
          "name": "appsactivity.activities.list",
          "request": {
            "url": "http://www.googleapis.com/appsactivity/v1/activities?drive.ancestorId=%7B%7D&drive.fileId=%7B%7D&groupingStrategy=%7B%7D&pageSize=%7B%7D&pageToken=%7B%7D&source=%7B%7D&userId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of activities visible to the current logged in user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43ad246a-709b-427a-9d89-ece9fc070542"
            }
          ]
        }
      ]
    }
  ]
}