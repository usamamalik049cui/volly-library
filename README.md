private fun apicall() {
        val Uri="https://some-random-api.ml/animal/dog"
        val queue = Volley.newRequestQueue(this)
        val jsonObjectRequest = JsonObjectRequest(
            Request.Method.Get,url, null,
            Response.Listener{
            Log.d("MainActivity", "Api call successful")

            },Response.ErrorListener
            {
                Log.d("MainActivity", "Api call failed")
            }
        )
    queue.add(JsonObjectRequest)
    }
