# GoogleSignInDemo
Simple Google Sign-In Android Application

```
GoogleSignInOptions gso = new GoogleSignInOptions.Builder(GoogleSignInOptions.DEFAULT_SIGN_IN)
                .requestScopes(new Scope(Scopes.PLUS_LOGIN))
                .requestEmail()
                .build();


mGoogleApiClient = new GoogleApiClient.Builder(this)
                .enableAutoManage(this /* FragmentActivity */, this /* OnConnectionFailedListener */)
                .addApi(Auth.GOOGLE_SIGN_IN_API, gso)
                .addApi(Plus.API)
                .build();
```

Reference sources:

[Try Sign-In for Android](https://developers.google.com/identity/sign-in/android/start)

[Add Sign-In to your existing app.](https://developers.google.com/identity/sign-in/android/start-integrating)
