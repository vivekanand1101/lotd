Packages to be used: ```net/http```, ```encoding/json``` and ```fmt``` for printing

The idea is to use ```http.Get``` from ```http``` module

Here is the code:

```
package main

import (
	"encoding/json"
	"fmt"
	"net/http"
)

type Github struct {
	Current_user_url                     string
	Current_user_authorizations_html_url string
	Authorizations_url                   string
	Code_search_url                      string
	Emails_url                           string
	Emojis_url                           string
	Events_url                           string
	Feeds_url                            string
	Followers_url                        string
	Following_url                        string
	Gists_url                            string
	hub_url                              string
	Issue_search_url                     string
	Issue_url                            string
	Keys_url                             string
	Notifications_url                    string
	Organization_repositories_url        string
	Organization_url                     string
	Public_gists_url                     string
	Rate_limit_url                       string
	Repository_url                       string
	Repository_search_url                string
	Current_user_repositories_url        string
	Starred_url                          string
	Starred_gists_url                    string
	Team_url                             string
	User_url                             string
	User_organizations_url               string
	User_repositories_url                string
	User_search_url                      string
}

func main() {
	res, err := http.Get("https://api.github.com/")
	if err != nil {
		fmt.Println("ERROR: ", err)
		return
	}
	fmt.Println("Response")
	github := Github{}
	defer res.Body.Close()
	json.NewDecoder(res.Body).Decode(&github)
	fmt.Println(github)
}

```

Point to be noted is, the first character should be capital of Github{} so that
it can be printed

