# Routing
## Simple React Router
- React Router has been broken into three packages: react-router, react-router-dom, and react-router-native.
- Links
our application needs a way to navigate between pages. If we were to create links using anchor elements, clicking on them would cause the whole page to reload. React Router provides a <Link> component to prevent that from happening. When clicking a <Link>, the URL will be updated and the rendered content will change without reloading the page.

```
/	---> the homepage
/roster	 ---> the team’s roster
/roster/:number	---> a profile for a player, using the player’s number
/schedule	---> the team’s schedule of games
```

## Hooks
React Router ships with a few hooks that let you access the state of the router and perform navigation from inside your components.

- useHistory
The useHistory hook gives you access to the history instance that you may use to navigate.
- useLocation
The useLocation hook returns the location object that represents the current URL. You can think about it like a useState that returns a new location whenever the URL changes.
- useParams
useParams returns an object of key/value pairs of URL parameters. Use it to access match.params of the current `<Route>.`
- useRouteMatch
The useRouteMatch hook attempts to match the current URL in the same way that a <Route> would. It’s mostly useful for getting access to the match data without actually rendering a <Route>.