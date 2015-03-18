# Documentation

Compass is a Jekyll theme designed with something very specific in mind: to be a simple and elegant personal landing page that can be easily deployed to [GitHub Pages](https://pages.github.com/).

## How to use Compass

1. Start by [installing Bundler](http://bundler.io) `gem install bundler`
2. [Fork the Compass repository](https://github.com/excentris/compass/fork)
3. Then run `bundle install` to get [Jekyll](http://jekyllrb.com) and all the dependencies.
4. Clone the repository you just forked: `git clone https://github.com/YOUR-USER/compass`
5. Edit `_config.yml` as needed.
6. Run the Jekyll server with `bundle exec jekyll serve`
7. Go to `http://localhost:4000`

## Deploy your site to GitHub Pages

If you want to use Compass as your personal landing page you can deploy your site to GitHub Pages as a [User Page](https://help.github.com/articles/user-organization-and-project-pages/#user--organization-pages). To do so, when you are done modifying your clone, you should rename your repository to `username.github.io` where username is your username. When GitHub builds the page it will be made available at `https://username.github.io`.

If you are planning on using a custom domain to direct to your site, modify the CNAME file as described [here](https://help.github.com/articles/adding-a-cname-file-to-your-repository/).

Check the [GitHub Pages Basics](https://help.github.com/categories/github-pages-basics/) for more information.

```json
//import org.json.simple.JSONObject;
  
  JSONObject obj=new JSONObject();
  obj.put("name","foo");
  obj.put("num",new Integer(100));
  obj.put("balance",new Double(1000.21));
  obj.put("is_vip",new Boolean(true));
  obj.put("nickname",null);
  System.out.print(obj);
  
  package main

import (
    "github.com/ant0ine/go-json-rest/rest"
    "log"
    "net/http"
)

func main() {
    api := rest.NewApi()
    api.Use(rest.DefaultDevStack...)
    api.SetApp(rest.AppSimple(func(w rest.ResponseWriter, r *rest.Request) {
        w.WriteJson(map[string]string{"Body": "Hello World!"})
    }))
    log.Fatal(http.ListenAndServe(":8080", api.MakeHandler()))
}
```
```html
// code for coloring
```
```js
// code for coloring
```
```css
// code for coloring
```
// etc.
