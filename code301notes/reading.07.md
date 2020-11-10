## What Google Learned About building Teams
Google did a lot of research into what makes a good team. The best teams in this study shared 2 qualities:

- Everyone in the group was allowed to speak and contribute an equal amount.
- People on the team had a high average social sensitivty, meaning they pick up on social queues well and are good at picking up on how others are feeling.

## SuperAgent
**SuperAgent**: light-weight progressive **ajax API** crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!

### Basic Requests
- A request can be initiated by invoking the appropriate method on the request object, then calling `.then()` (or `.end()` or `await()` to send the request
- **EX:** `request
   .get('/search')
   .then(res => {
      // res.body, res.headers, res.status
   })
   .catch(err => {
      // err.message, err.response
   });`

### For the API keys, go to your folder!
[<-- Back](301readingnotes.md) [Back to Home](README.md)
