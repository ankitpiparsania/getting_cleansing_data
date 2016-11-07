



<!DOCTYPE html>
<html lang="en" class=" is-copy-enabled is-u2f-enabled">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    

    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/frameworks-119461b8a22c3dc631a815795aa9d7f436fe38386cd99a1ca106fd2798f159aa.css" integrity="sha256-EZRhuKIsPcYxqBV5WqnX9Db+ODhs2ZocoQb9J5jxWao=" media="all" rel="stylesheet" />
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github-fb3f5ff93b051ac1e6146d6a27dc2f57e11f1b9b36a7f15bbd84aacdb65ec3a8.css" integrity="sha256-+z9f+TsFGsHmFG1qJ9wvV+EfG5s2p/FbvYSqzbZew6g=" media="all" rel="stylesheet" />
    
    
    
    

    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    <meta name="viewport" content="width=device-width">
    
    <title>getting_cleaning_data/codebook.md at master · coursera-datascience/getting_cleaning_data</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" href="/apple-touch-icon.png">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="/apple-touch-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="/apple-touch-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="/apple-touch-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="/apple-touch-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon-180x180.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="https://avatars1.githubusercontent.com/u/7218917?v=3&amp;s=400" name="twitter:image:src" /><meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="coursera-datascience/getting_cleaning_data" name="twitter:title" /><meta content="Contribute to getting_cleaning_data development by creating an account on GitHub." name="twitter:description" />
      <meta content="https://avatars1.githubusercontent.com/u/7218917?v=3&amp;s=400" property="og:image" /><meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="coursera-datascience/getting_cleaning_data" property="og:title" /><meta content="https://github.com/coursera-datascience/getting_cleaning_data" property="og:url" /><meta content="Contribute to getting_cleaning_data development by creating an account on GitHub." property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="web-socket" href="wss://live.github.com/_sockets/MjAzNjQ3MDM6NzM0YzYxYWNkNmMxMzZiZjU2MDM4ODY5NWFjYzEyNDk6YTM4NTg2MDljNjkzYTM0NTFmNGVlZGVjMDkzNTZmYjFmYzFkODk1MDc1MDhiYjI5MDhlZTgwMDFhYjAyZjlmNw==--4e1760e168fbb08bb073c8a36bf54dd24fa47bd4">
    <meta name="pjax-timeout" content="1000">
    <link rel="sudo-modal" href="/sessions/sudo_modal">
    <meta name="request-id" content="49CABA9E:2272:3CE85A7:58200DD4" data-pjax-transient>

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>

    <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
<meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-analytics" content="UA-3769691-2">

<meta content="collector.githubapp.com" name="octolytics-host" /><meta content="github" name="octolytics-app-id" /><meta content="49CABA9E:2272:3CE85A7:58200DD4" name="octolytics-dimension-request_id" /><meta content="20364703" name="octolytics-actor-id" /><meta content="ankitpiparsania" name="octolytics-actor-login" /><meta content="7ce784bf8efac374fdb06ab50879d918d0e83c3cabf9bcbce03676d739a7869c" name="octolytics-actor-hash" />
<meta content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" name="analytics-location" />



  <meta class="js-ga-set" name="dimension1" content="Logged In">



        <meta name="hostname" content="github.com">
    <meta name="user-login" content="ankitpiparsania">

        <meta name="expected-hostname" content="github.com">
      <meta name="js-proxy-site-detection-payload" content="MTJlM2I0MzNlOWExOTczZjAxNzYzNzk5YzgzM2U4YWNiODFhNDk4MjE5ZTA2MzQxMmQ0MDEzYTNmMTZkMzVjYXx7InJlbW90ZV9hZGRyZXNzIjoiNzMuMjAyLjE4Ni4xNTgiLCJyZXF1ZXN0X2lkIjoiNDlDQUJBOUU6MjI3MjozQ0U4NUE3OjU4MjAwREQ0IiwidGltZXN0YW1wIjoxNDc4NDk1NzAwLCJob3N0IjoiZ2l0aHViLmNvbSJ9">


      <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#4078c0">
      <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

    <meta name="html-safe-nonce" content="9b0a74484fdcfc8ecf673a736c4f638564bee8df">
    <meta content="6f424b7a27ed88db5c8f89804e221d29c0bfd54c" name="form-nonce" />

    <meta http-equiv="x-pjax-version" content="4274452f598450a3d9b254e0c1032f59">
    

      
  <meta name="description" content="Contribute to getting_cleaning_data development by creating an account on GitHub.">
  <meta name="go-import" content="github.com/coursera-datascience/getting_cleaning_data git https://github.com/coursera-datascience/getting_cleaning_data.git">

  <meta content="7218917" name="octolytics-dimension-user_id" /><meta content="coursera-datascience" name="octolytics-dimension-user_login" /><meta content="19505299" name="octolytics-dimension-repository_id" /><meta content="coursera-datascience/getting_cleaning_data" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="19505299" name="octolytics-dimension-repository_network_root_id" /><meta content="coursera-datascience/getting_cleaning_data" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/coursera-datascience/getting_cleaning_data/commits/master.atom" rel="alternate" title="Recent Commits to getting_cleaning_data:master" type="application/atom+xml">


      <link rel="canonical" href="https://github.com/coursera-datascience/getting_cleaning_data/blob/master/codebook.md" data-pjax-transient>
  </head>


  <body class="logged-in  env-production windows vis-public page-blob">
    <div id="js-pjax-loader-bar" class="pjax-loader-bar"><div class="progress"></div></div>
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>

    
    
    



        <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" data-ga-click="Header, go to dashboard, icon:logo">
  <svg aria-hidden="true" class="octicon octicon-mark-github" height="28" version="1.1" viewBox="0 0 16 16" width="28"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path></svg>
</a>


        <div class="header-search scoped-search site-scoped-search js-site-search" role="search">
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/coursera-datascience/getting_cleaning_data/search" class="js-site-search-form" data-scoped-search-url="/coursera-datascience/getting_cleaning_data/search" data-unscoped-search-url="/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <label class="form-control header-search-wrapper js-chromeless-input-container">
      <div class="header-search-scope">This repository</div>
      <input type="text"
        class="form-control header-search-input js-site-search-focus js-site-search-field is-clearable"
        data-hotkey="s"
        name="q"
        placeholder="Search"
        aria-label="Search this repository"
        data-unscoped-placeholder="Search GitHub"
        data-scoped-placeholder="Search"
        autocapitalize="off">
    </label>
</form></div>


      <ul class="header-nav float-left" role="navigation">
        <li class="header-nav-item">
          <a href="/pulls" aria-label="Pull requests you created" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:pulls context:user" data-hotkey="g p" data-selected-links="/pulls /pulls/assigned /pulls/mentioned /pulls">
            Pull requests
</a>        </li>
        <li class="header-nav-item">
          <a href="/issues" aria-label="Issues you created" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:issues context:user" data-hotkey="g i" data-selected-links="/issues /issues/assigned /issues/mentioned /issues">
            Issues
</a>        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com/" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
      </ul>

    
<ul class="header-nav user-nav float-right" id="user-links">
  <li class="header-nav-item">
    

  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link tooltipped tooltipped-s js-menu-target" href="/new"
       aria-label="Create new…"
       data-ga-click="Header, create new, icon:add">
      <svg aria-hidden="true" class="octicon octicon-plus float-left" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 9H7v5H5V9H0V7h5V2h2v5h5z"></path></svg>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <ul class="dropdown-menu dropdown-menu-sw">
        
<a class="dropdown-item" href="/new" data-ga-click="Header, create new repository">
  New repository
</a>

  <a class="dropdown-item" href="/new/import" data-ga-click="Header, import a repository">
    Import repository
  </a>

<a class="dropdown-item" href="https://gist.github.com/" data-ga-click="Header, create new gist">
  New gist
</a>

  <a class="dropdown-item" href="/organizations/new" data-ga-click="Header, create new organization">
    New organization
  </a>



  <div class="dropdown-divider"></div>
  <div class="dropdown-header">
    <span title="coursera-datascience/getting_cleaning_data">This repository</span>
  </div>
    <a class="dropdown-item" href="/coursera-datascience/getting_cleaning_data/issues/new" data-ga-click="Header, create new issue">
      New issue
    </a>

      </ul>
    </div>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name tooltipped tooltipped-sw js-menu-target" href="/ankitpiparsania"
       aria-label="View profile and more"
       data-ga-click="Header, show menu, icon:avatar">
      <img alt="@ankitpiparsania" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/20364703?v=3&amp;s=40" width="20" />
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <div class="dropdown-menu dropdown-menu-sw">
        <div class="dropdown-header header-nav-current-user css-truncate">
          Signed in as <strong class="css-truncate-target">ankitpiparsania</strong>
        </div>

        <div class="dropdown-divider"></div>

        <a class="dropdown-item" href="/ankitpiparsania" data-ga-click="Header, go to profile, text:your profile">
          Your profile
        </a>
        <a class="dropdown-item" href="/ankitpiparsania?tab=stars" data-ga-click="Header, go to starred repos, text:your stars">
          Your stars
        </a>
        <a class="dropdown-item" href="/explore" data-ga-click="Header, go to explore, text:explore">
          Explore
        </a>
          <a class="dropdown-item" href="/integrations" data-ga-click="Header, go to integrations, text:integrations">
            Integrations
          </a>
        <a class="dropdown-item" href="https://help.github.com" data-ga-click="Header, go to help, text:help">
          Help
        </a>

        <div class="dropdown-divider"></div>

        <a class="dropdown-item" href="/settings/profile" data-ga-click="Header, go to settings, icon:settings">
          Settings
        </a>

        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/logout" class="logout-form" data-form-nonce="6f424b7a27ed88db5c8f89804e221d29c0bfd54c" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="8sjMM3S3DFU9Adix61wg8aw6a9rUIgXM5Dc0y5n9LOJiNg/7xjGWtnUMv0GLTZbBrkVUdEnhiYp2tL2MGHTotw==" /></div>
          <button type="submit" class="dropdown-item dropdown-signout" data-ga-click="Header, sign out, icon:logout">
            Sign out
          </button>
</form>      </div>
    </div>
  </li>
</ul>


    
  </div>
</div>


      


    <div id="start-of-content" class="accessibility-aid"></div>

      <div id="js-flash-container">
</div>


    <div role="main">
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode">
    <div id="js-repo-pjax-container" data-pjax-container>
      
<div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav">
  <div class="container repohead-details-container">

    

<ul class="pagehead-actions">

  <li>
        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-form-nonce="6f424b7a27ed88db5c8f89804e221d29c0bfd54c" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="nRpMPpTGsVFY/iiG4EOtQ9CToWnRPWzTihHb77FlnC3j6jyUs0QVJxkgKfYYW54bx5I+v2FL1GGQ1nY+OHi3YA==" /></div>      <input class="form-control" id="repository_id" name="repository_id" type="hidden" value="19505299" />

        <div class="select-menu js-menu-container js-select-menu">
          <a href="/coursera-datascience/getting_cleaning_data/subscription"
            class="btn btn-sm btn-with-count select-menu-button js-menu-target" role="button" tabindex="0" aria-haspopup="true"
            data-ga-click="Repository, click Watch settings, action:blob#show">
            <span class="js-select-button">
              <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"></path></svg>
              Watch
            </span>
          </a>
          <a class="social-count js-social-count"
            href="/coursera-datascience/getting_cleaning_data/watchers"
            aria-label="1 user is watching this repository">
            1
          </a>

        <div class="select-menu-modal-holder">
          <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
            <div class="select-menu-header js-navigation-enable" tabindex="-1">
              <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
              <span class="select-menu-title">Notifications</span>
            </div>

              <div class="select-menu-list js-navigation-container" role="menu">

                <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input checked="checked" id="do_included" name="do" type="radio" value="included" />
                    <span class="select-menu-item-heading">Not watching</span>
                    <span class="description">Be notified when participating or @mentioned.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"></path></svg>
                      Watch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input id="do_subscribed" name="do" type="radio" value="subscribed" />
                    <span class="select-menu-item-heading">Watching</span>
                    <span class="description">Be notified of all conversations.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"></path></svg>
                      Unwatch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input id="do_ignore" name="do" type="radio" value="ignore" />
                    <span class="select-menu-item-heading">Ignoring</span>
                    <span class="description">Never be notified.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-mute" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8 2.81v10.38c0 .67-.81 1-1.28.53L3 10H1c-.55 0-1-.45-1-1V7c0-.55.45-1 1-1h2l3.72-3.72C7.19 1.81 8 2.14 8 2.81zm7.53 3.22l-1.06-1.06-1.97 1.97-1.97-1.97-1.06 1.06L11.44 8 9.47 9.97l1.06 1.06 1.97-1.97 1.97 1.97 1.06-1.06L13.56 8l1.97-1.97z"></path></svg>
                      Stop ignoring
                    </span>
                  </div>
                </div>

              </div>

            </div>
          </div>
        </div>
</form>
  </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/coursera-datascience/getting_cleaning_data/unstar" class="starred" data-form-nonce="6f424b7a27ed88db5c8f89804e221d29c0bfd54c" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="12hO+f+Nyevp/dwqu/AZ3wA7tdYmHZ3wwsQfjxuKaQ09kruGXWzQzUdAegJdchOURGhu1P1D1LaKQnQg81uWgA==" /></div>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Unstar this repository" title="Unstar coursera-datascience/getting_cleaning_data"
        data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar">
        <svg aria-hidden="true" class="octicon octicon-star" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74z"></path></svg>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/coursera-datascience/getting_cleaning_data/stargazers"
           aria-label="0 users starred this repository">
          0
        </a>
</form>
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/coursera-datascience/getting_cleaning_data/star" class="unstarred" data-form-nonce="6f424b7a27ed88db5c8f89804e221d29c0bfd54c" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="PG1R7GkpK14HS/7y07gHp8iVoRDQSBLM79f9pkpQCHE68CgaXdjB1rOHBek39CFu1+IScaAPS2RvB79uFOAniA==" /></div>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Star this repository" title="Star coursera-datascience/getting_cleaning_data"
        data-ga-click="Repository, click star button, action:blob#show; text:Star">
        <svg aria-hidden="true" class="octicon octicon-star" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74z"></path></svg>
        Star
      </button>
        <a class="social-count js-social-count" href="/coursera-datascience/getting_cleaning_data/stargazers"
           aria-label="0 users starred this repository">
          0
        </a>
</form>  </div>

  </li>

  <li>
          <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/coursera-datascience/getting_cleaning_data/fork" class="btn-with-count" data-form-nonce="6f424b7a27ed88db5c8f89804e221d29c0bfd54c" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="SLTbYNiPD+qHT1bGOPU7Z7Nvw5cyL6YtFYSliqeD3kzFcnGTFBkPdAfMMqx7iaBx4/byR6mOLATt7nObXWYggQ==" /></div>
            <button
                type="submit"
                class="btn btn-sm btn-with-count"
                data-ga-click="Repository, show fork modal, action:blob#show; text:Fork"
                title="Fork your own copy of coursera-datascience/getting_cleaning_data to your account"
                aria-label="Fork your own copy of coursera-datascience/getting_cleaning_data to your account">
              <svg aria-hidden="true" class="octicon octicon-repo-forked" height="16" version="1.1" viewBox="0 0 10 16" width="10"><path d="M8 1a1.993 1.993 0 0 0-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 0 0 2 1a1.993 1.993 0 0 0-1 3.72V6.5l3 3v1.78A1.993 1.993 0 0 0 5 15a1.993 1.993 0 0 0 1-3.72V9.5l3-3V4.72A1.993 1.993 0 0 0 8 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"></path></svg>
              Fork
            </button>
</form>
    <a href="/coursera-datascience/getting_cleaning_data/network" class="social-count"
       aria-label="0 users are forked this repository">
      0
    </a>
  </li>
</ul>

    <h1 class="public ">
  <svg aria-hidden="true" class="octicon octicon-repo" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"></path></svg>
  <span class="author" itemprop="author"><a href="/coursera-datascience" class="url fn" rel="author">coursera-datascience</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a href="/coursera-datascience/getting_cleaning_data" data-pjax="#js-repo-pjax-container">getting_cleaning_data</a></strong>

</h1>

  </div>
  <div class="container">
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
     role="navigation"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/coursera-datascience/getting_cleaning_data" aria-selected="true" class="js-selected-navigation-item selected reponav-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /coursera-datascience/getting_cleaning_data" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-code" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"></path></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a href="/coursera-datascience/getting_cleaning_data/issues" class="js-selected-navigation-item reponav-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /coursera-datascience/getting_cleaning_data/issues" itemprop="url">
        <svg aria-hidden="true" class="octicon octicon-issue-opened" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7s-2.56 5.7-5.7 5.7A5.71 5.71 0 0 1 1.3 8c0-3.14 2.56-5.7 5.7-5.7zM7 1C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7-3.14-7-7-7zm1 3H6v5h2V4zm0 6H6v2h2v-2z"></path></svg>
        <span itemprop="name">Issues</span>
        <span class="counter">0</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/coursera-datascience/getting_cleaning_data/pulls" class="js-selected-navigation-item reponav-item" data-hotkey="g p" data-selected-links="repo_pulls /coursera-datascience/getting_cleaning_data/pulls" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-git-pull-request" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0 0 10 15a1.993 1.993 0 0 0 1-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v6.56A1.993 1.993 0 0 0 2 15a1.993 1.993 0 0 0 1-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"></path></svg>
      <span itemprop="name">Pull requests</span>
      <span class="counter">0</span>
      <meta itemprop="position" content="3">
</a>  </span>

  <a href="/coursera-datascience/getting_cleaning_data/projects" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /coursera-datascience/getting_cleaning_data/projects">
    <svg class="octicon" aria-hidden="true" version="1.1" width="15" height="16" viewBox="0 0 15 16">
      <path d="M1 15h13V1H1v14zM15 1v14a1 1 0 0 1-1 1H1a1 1 0 0 1-1-1V1a1 1 0 0 1 1-1h13a1 1 0 0 1 1 1zm-4.41 11h1.82c.59 0 .59-.41.59-1V3c0-.59 0-1-.59-1h-1.82C10 2 10 2.41 10 3v8c0 .59 0 1 .59 1zm-4-2h1.82C9 10 9 9.59 9 9V3c0-.59 0-1-.59-1H6.59C6 2 6 2.41 6 3v6c0 .59 0 1 .59 1zM2 13V3c0-.59 0-1 .59-1h1.82C5 2 5 2.41 5 3v10c0 .59 0 1-.59 1H2.59C2 14 2 13.59 2 13z"></path>
    </svg>
    Projects
    <span class="counter">0</span>
</a>
    <a href="/coursera-datascience/getting_cleaning_data/wiki" class="js-selected-navigation-item reponav-item" data-hotkey="g w" data-selected-links="repo_wiki /coursera-datascience/getting_cleaning_data/wiki">
      <svg aria-hidden="true" class="octicon octicon-book" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M3 5h4v1H3V5zm0 3h4V7H3v1zm0 2h4V9H3v1zm11-5h-4v1h4V5zm0 2h-4v1h4V7zm0 2h-4v1h4V9zm2-6v9c0 .55-.45 1-1 1H9.5l-1 1-1-1H2c-.55 0-1-.45-1-1V3c0-.55.45-1 1-1h5.5l1 1 1-1H15c.55 0 1 .45 1 1zm-8 .5L7.5 3H2v9h6V3.5zm7-.5H9.5l-.5.5V12h6V3z"></path></svg>
      Wiki
</a>

  <a href="/coursera-datascience/getting_cleaning_data/pulse" class="js-selected-navigation-item reponav-item" data-selected-links="pulse /coursera-datascience/getting_cleaning_data/pulse">
    <svg aria-hidden="true" class="octicon octicon-pulse" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M11.5 8L8.8 5.4 6.6 8.5 5.5 1.6 2.38 8H0v2h3.6l.9-1.8.9 5.4L9 8.5l1.6 1.5H14V8z"></path></svg>
    Pulse
</a>
  <a href="/coursera-datascience/getting_cleaning_data/graphs" class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors /coursera-datascience/getting_cleaning_data/graphs">
    <svg aria-hidden="true" class="octicon octicon-graph" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"></path></svg>
    Graphs
</a>

</nav>

  </div>
</div>

<div class="container new-discussion-timeline experiment-repo-nav">
  <div class="repository-content">

    

<a href="/coursera-datascience/getting_cleaning_data/blob/2c8509901dfed3ab04ac67dee9da97a6bb88f891/codebook.md" class="d-none js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:4dcfd8cca03c1fe6ada747c8e213481f -->

<div class="file-navigation js-zeroclipboard-container">
  
<div class="select-menu branch-select-menu js-menu-container js-select-menu float-left">
  <button class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    
    type="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <i>Branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
        <span class="select-menu-title">Switch branches/tags</span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="form-control js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Filter branches/tags" class="js-select-menu-tab" role="tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab" role="tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches" role="menu">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/coursera-datascience/getting_cleaning_data/blob/master/codebook.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"></path></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                master
              </span>
            </a>
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

  <div class="BtnGroup float-right">
    <a href="/coursera-datascience/getting_cleaning_data/find/master"
          class="js-pjax-capture-input btn btn-sm BtnGroup-item"
          data-pjax
          data-hotkey="t">
      Find file
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm BtnGroup-item tooltipped tooltipped-s" data-copied-hint="Copied!" type="button">Copy path</button>
  </div>
  <div class="breadcrumb js-zeroclipboard-target">
    <span class="repo-root js-repo-root"><span class="js-path-segment"><a href="/coursera-datascience/getting_cleaning_data"><span>getting_cleaning_data</span></a></span></span><span class="separator">/</span><strong class="final-path">codebook.md</strong>
  </div>
</div>


  <div class="commit-tease">
      <span class="float-right">
        <a class="commit-tease-sha" href="/coursera-datascience/getting_cleaning_data/commit/033ff5675a05ae05c9fd3facf51541757ca9112a" data-pjax>
          033ff56
        </a>
        <relative-time datetime="2014-05-12T21:33:03Z">May 12, 2014</relative-time>
      </span>
      <div>
        <img alt="@coursera-datascience" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/7218917?v=3&amp;s=40" width="20" />
        <a href="/coursera-datascience" class="user-mention" rel="author">coursera-datascience</a>
          <a href="/coursera-datascience/getting_cleaning_data/commit/033ff5675a05ae05c9fd3facf51541757ca9112a" class="message" data-pjax="true" title="Final">Final</a>
      </div>

    <div class="commit-tease-contributors">
      <button type="button" class="btn-link muted-link contributors-toggle" data-facebox="#blob_contributors_box">
        <strong>1</strong>
         contributor
      </button>
      
    </div>

    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header" data-facebox-id="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list" data-facebox-id="facebox-description">
          <li class="facebox-user-list-item">
            <img alt="@coursera-datascience" height="24" src="https://avatars2.githubusercontent.com/u/7218917?v=3&amp;s=48" width="24" />
            <a href="/coursera-datascience">coursera-datascience</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file">
  <div class="file-header">
  <div class="file-actions">

    <div class="BtnGroup">
      <a href="/coursera-datascience/getting_cleaning_data/raw/master/codebook.md" class="btn btn-sm BtnGroup-item" id="raw-url">Raw</a>
        <a href="/coursera-datascience/getting_cleaning_data/blame/master/codebook.md" class="btn btn-sm js-update-url-with-hash BtnGroup-item">Blame</a>
      <a href="/coursera-datascience/getting_cleaning_data/commits/master/codebook.md" class="btn btn-sm BtnGroup-item" rel="nofollow">History</a>
    </div>

        <a class="btn-octicon tooltipped tooltipped-nw"
           href="https://windows.github.com"
           aria-label="Open this file in GitHub Desktop"
           data-ga-click="Repository, open with desktop, type:windows">
            <svg aria-hidden="true" class="octicon octicon-device-desktop" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M15 2H1c-.55 0-1 .45-1 1v9c0 .55.45 1 1 1h5.34c-.25.61-.86 1.39-2.34 2h8c-1.48-.61-2.09-1.39-2.34-2H15c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm0 9H1V3h14v8z"></path></svg>
        </a>

        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/coursera-datascience/getting_cleaning_data/edit/master/codebook.md" class="inline-form js-update-url-with-hash" data-form-nonce="6f424b7a27ed88db5c8f89804e221d29c0bfd54c" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="d3idV2+AtfUGxpETNVAiFGGMhkDAipODTuzLrSDMHVRORmAoQ17w/kD+C+uwvNppgb7WHDr8ACYRPuXmwI8ViA==" /></div>
          <button class="btn-octicon tooltipped tooltipped-nw" type="submit"
            aria-label="Fork this project and edit the file" data-hotkey="e" data-disable-with>
            <svg aria-hidden="true" class="octicon octicon-pencil" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 0 1 1.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"></path></svg>
          </button>
</form>        <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/coursera-datascience/getting_cleaning_data/delete/master/codebook.md" class="inline-form" data-form-nonce="6f424b7a27ed88db5c8f89804e221d29c0bfd54c" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="nlI8ASyQynnsr4wlF2Qty0fnR+8Wjd3PvZTnpdYzUrCT4xTncIBAVSzhMmFsdRalwhH7ngwhpQV+I8S6sg3uWQ==" /></div>
          <button class="btn-octicon btn-octicon-danger tooltipped tooltipped-nw" type="submit"
            aria-label="Fork this project and delete the file" data-disable-with>
            <svg aria-hidden="true" class="octicon octicon-trashcan" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"></path></svg>
          </button>
</form>  </div>

  <div class="file-info">
      228 lines (202 sloc)
      <span class="file-info-divider"></span>
    15.9 KB
  </div>
</div>

  
  <div id="readme" class="readme blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-samsung-galaxy-s-smartphone-data-codebookmay-2014" class="anchor" href="#samsung-galaxy-s-smartphone-data-codebookmay-2014" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Samsung Galaxy S Smartphone Data CodeBookMay 2014</h1>

<h4><a id="user-content-coursera-getting-clearning-data-project" class="anchor" href="#coursera-getting-clearning-data-project" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Coursera Getting Clearning Data Project</h4>

<h2><a id="user-content-i-introduction" class="anchor" href="#i-introduction" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>I. Introduction</h2>

<p>This file describes the data, the variables, and the work that has been performed to clean up the borrowed dataset of Samsung Galaxy S Smartphone data.</p>

<h2><a id="user-content-ii-data-set-description" class="anchor" href="#ii-data-set-description" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>II. Data Set Description</h2>

<p>The borrowed dataset was originally collected from an experiment, which was carried out with a group of 30 volunteers of 19-48 years. Wearing Samsung Galaxy S II smartphone on the waist, each participant performed six activities such as walking, walking upstairs, walking downstairs, sitting, standing, and laying. The phone's embedded accelerometer and gyroscope captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments were video-recorded to label the data manually. The obtained dataset then was randomly partitioned into two sets, where 70% of the participants was selected for generating the training data and 30% the test data. </p>

<h3><a id="user-content-files-included-in-the-original-dataset" class="anchor" href="#files-included-in-the-original-dataset" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Files included in the original dataset</h3>

<p>The original dataset, which was in the form of a compression file, was downloaded from <a href="https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip">https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip</a>.  The extracted dataset folder ("UCI HAR Dataset") contains four text files and two sub-directory folders as shown below:</p>

<p>[UCI HAR Dataset]
</p><dd> -- activity_labels.txt </dd>
<dd> -- feactures_info.txt </dd>
<dd> -- features.txt </dd>
<dd> -- README.txt </dd>
<dd> -- [test]      </dd>
<dd> -- [train]     </dd><p></p>

<p>The 'activity_labels.txt' file links the class labels with their activity name.
The 'features_info.txt' file provides information about the variables used on the feature vector.
The 'features.txt' file lists all features(variables).</p>

<p>In each sub-directory folder of 'test' and 'train', there are three text files and one sub_folder:</p>

<p>[test]<br>
</p><dd> -- subject_test.txt </dd>
<dd> -- X_test.txt </dd>
<dd> -- y_test.txt </dd>
<dd> -- [Inertial Signals]    </dd>
[train]<br>
<dd> -- subject_train.txt </dd>
<dd> -- X_train.txt </dd>
<dd> -- y_train.txt </dd>
<dd> -- [Inertial Signals]   </dd><p></p>

<p>The 'subject_test.txt' and 'subject_train.txt' files provide information regarding subjects. Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30.
The 'X_test.txt' and 'X_train.txt' files contain the test and training set data.
The 'y_test.txt' and 'y_train.txt' files conatin the test and training data labels.
The 'Inertial Signals/total_acc_x_train.txt' file contains the acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis.
The 'Inertial Signals/body_acc_x_train.txt' file contains the body acceleration signal obtained by subtracting the gravity from the total acceleration.
The 'Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second.</p>

<p>The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. </p>

<h3><a id="user-content-attributes" class="anchor" href="#attributes" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Attributes</h3>

<p>Each record in the original dataset contained the following information:</p>

<ul>
<li>Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration</li>
<li>Triaxial Angular velocity from the gyroscope</li>
<li>A 561-feature vector with time and frequency domain variables</li>
<li>Its activity label</li>
<li>An identifier of the subject who carried out the experiment</li>
</ul>

<h2><a id="user-content-iii-variables-in-the-original-data-set" class="anchor" href="#iii-variables-in-the-original-data-set" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>III. Variables in the Original Data Set</h2>

<p>The variables in the original dataset come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz.</p>

<p>Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag).</p>

<p>Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals).</p>

<p>These signals were used to estimate variables of the feature vector for each pattern:
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.</p>

<h2><a id="user-content-iv-transformations" class="anchor" href="#iv-transformations" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>IV. Transformations</h2>

<p>For the data cleaning, a R script is created. This 'run_analysis.R' script contains five functions as listed below:</p>

<table border="1">
<tbody><tr>
<th>Function Name</th><th>Goal/Task</th><th width="15%">Files Used</th><th>Output File</th><th>Command</th>
</tr>
<tr>
<th valign="top">SimpleMerge</th>
<td valign="top">Merge the training and the test sets into one data set.<br>
1) Subject ID (subject_test.txt and subject_train.txt) is merged as the first column of the merged data set.<br>
2) Activity type (y_test.txt and y_train.txt) is merged as the second column of the merged data set.<br>
3) Descriptive activity information is copied from the activity_labels.txt file.</td>
<td valign="top">1) X_test.txt<br>2) y_test.txt<br>3) X_train.txt<br>4) y_train.txt<br>5) subject_test.txt <br>6) subject_train.txt<br> 7) features.txt</td>
<td valign="top">SimpleMerge.txt<br> (563 variables) <br> (10299 cases)</td>
<td valign="top">SimpleMerge()</td>
</tr>
<tr>
<th valign="top">MeanStdMerge</th>
<td valign="top">Extract only the measurments on the mean and standard deviation (as well as subject id and activity type) for each measurement.<br>
1) At the time of this function call, if SimpleMerge.txt does not exist, this function calls the SimpleMerge() function and creates the SimpleMerge.txt file.<br>
2) If the SimpleMerge.txt file does exist, however, this function reads the file, pattern matches the column names for mean and standard deviation using 'grepl' (as well as 'subjectid' and 'activitytype'), and subset only the matched columns.</td>
<td valign="top">1) SimpleMerge.txt</td>
<td valign="top">MeanStdMerge.txt<br> (68 variables) <br> (10299 cases)</td>
<td valign="top">MeanStdMerge()</td>
</tr>
<tr>
<th valign="top">DesVarMerge</th>
<td valign="top">Label the data set with descriptive variable names.<br>
1) At the time of this function call, if MeanStdMerge.txt does not exist, this function calls the MeanStdMerge() function and creates the MeanStdMerge.txt file.<br>
2) If the MeanStdMerge.txt file does exist, however, this function reads the file and replace the variable names (column headings) descriptive variable names.</td>
<td valign="top">1) MeanStdMerge.txt</td>
<td valign="top">DesVarMerge.txt<br> (68 variables) <br> (10299 cases)</td>
<td valign="top">DesVarMerge()</td>
</tr>
<tr>
<th valign="top">DesActMerge</th>
<td valign="top">Replace activity numbers with descriptive activity names.<br>
1) Descriptive activity information is copied from the activity_labels.txt file.<br>
2) At the time of this function call, if desVarMerge.txt does not exist, this function calls the desVarMerge() function and creates the desVarMerge.txt file.<br>
3) If the desVarMerge.txt file does exist, however, this function reads the file and replace the values of the activity column from numeric code to descriptive activity types.</td>
<td valign="top">1) activity_labels.txt <br> 2) DesVarMerge.txt</td>
<td valign="top">DesActMerge.txt<br> (68 variables) <br> (10299 cases)</td>
<td valign="top">DesActMerge()</td>
</tr>
<tr><th valign="top">AvgMerge</th>
<td valign="top">Create a new tidy data set with the average of each variable for each activity and each subject.<br>
1) At the time of this function call, if desActMerge.txt does not exist, this function calls the desActMerge() function and creates the desActMerge.txt file.<br>
2) If the desActMerge.txt file does exist, however, this function reads the file, loop through each subject and each activity type, and calculate average value of each variable in the dataset (of course, excluding the subject id and activity type column).</td>
<td valign="top">1) activity_labels.txt <br> 2) DesActMerge.txt</td>
<td valign="top">AvgMerge.txt<br> (68 variables) <br> (180 cases)</td>
<td valign="top">AvgMerge()</td>
</tr>
</tbody></table>

<h2><a id="user-content-v-variables-in-the-tidy-data-set" class="anchor" href="#v-variables-in-the-tidy-data-set" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>V. Variables in the Tidy Data Set</h2>

<p>The tidy data set contains a total of 68 variables. </p>

<h4><a id="user-content-variable-names" class="anchor" href="#variable-names" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Variable Names</h4>

<p>As a part of the data cleaning process (DesVarMerge function), variable names are changed so that they could be more intuitive. The R code changed variable names in the following systematic way:</p>

<table>
<tbody><tr><th>From</th><th>To</th><th>Description</th></tr>
<tr><td>[no variable name]</td><td>subjectid</td><td>individual participant's identification number</td></tr>
<tr><td valign="top">[no variable name]</td><td valign="top">activitytype</td><td>type of activity that participant practiced<br>
                                                1) WALKING<br>
                                                2) WALKING_UPSTAIRS<br>
                                                3) WALKING_DOWNSTAIRS<br>
                                                4) SITTING5) STANDING<br>
                                                6) LAYING
</td></tr>
<tr><td>the prefix 't'</td><td>time</td><td>time domain signals</td></tr>
<tr><td>the prefix 'f'</td><td>frequency</td><td>frequency domain signals</td></tr>
<tr><td>Acc</td><td>acceleration</td><td>data from the accelerometer signals</td></tr>
<tr><td>Gyro</td><td>gyroscope</td><td>data from the gyroscope signals</td></tr>
<tr><td>Mag</td><td>magnitude</td><td>magnitude of signals</td></tr>
<tr><td>mean()</td><td>mean</td><td>mean value</td></tr>
<tr><td>std()</td><td>standarddeviation</td><td>standard deviation</td></tr>
</tbody></table>

<p><br>
Additionally, a set of parentheses is replaced by a dot, unless the set is located in the end of the variable name; in that case, parentheses are simply removed. Commas are replaced by a dot as well. All upper case letters are changed to lower case letters. Finally, to indicate that variables other than the subject id and activitytype are the average of each activity and each subject, the prefix of "average" is added to the variable names. The following table lists the variable column location, variable name, and length of variable. 
<br><br></p>

<table><thead>
<tr>
<th>Variable Column Location</th>
<th>Variable Name</th>
<th>Class</th>
<th>Length</th>
</tr>
</thead><tbody>
<tr>
<td>1</td>
<td>subjectid</td>
<td>integer</td>
<td>1</td>
</tr>
<tr>
<td>2</td>
<td>activitytype</td>
<td>factor</td>
<td>1</td>
</tr>
<tr>
<td>3</td>
<td>average.timebodyacceleration.mean.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>4</td>
<td>average.timebodyacceleration.mean.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>5</td>
<td>average.timebodyacceleration.mean.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>6</td>
<td>average.timebodyacceleration.standarddeviation.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>7</td>
<td>average.timebodyacceleration.standarddeviation.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>8</td>
<td>average.timebodyacceleration.standarddeviation.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>9</td>
<td>average.timegravityacceleration.mean.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>10</td>
<td>average.timegravityacceleration.mean.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>11</td>
<td>average.timegravityacceleration.mean.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>12</td>
<td>average.timegravityacceleration.standarddeviation.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>13</td>
<td>average.timegravityacceleration.standarddeviation.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>14</td>
<td>average.timegravityacceleration.standarddeviation.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>15</td>
<td>average.timebodyaccelerationjerk.mean.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>16</td>
<td>average.timebodyaccelerationjerk.mean.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>17</td>
<td>average.timebodyaccelerationjerk.mean.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>18</td>
<td>average.timebodyaccelerationjerk.standarddeviation.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>19</td>
<td>average.timebodyaccelerationjerk.standarddeviation.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>20</td>
<td>average.timebodyaccelerationjerk.standarddeviation.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>21</td>
<td>average.timebodygyroscope.mean.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>22</td>
<td>average.timebodygyroscope.mean.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>23</td>
<td>average.timebodygyroscope.mean.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>24</td>
<td>average.timebodygyroscope.standarddeviation.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>25</td>
<td>average.timebodygyroscope.standarddeviation.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>26</td>
<td>average.timebodygyroscope.standarddeviation.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>27</td>
<td>average.timebodygyroscopejerk.mean.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>28</td>
<td>average.timebodygyroscopejerk.mean.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>29</td>
<td>average.timebodygyroscopejerk.mean.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>30</td>
<td>average.timebodygyroscopejerk.standarddeviation.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>31</td>
<td>average.timebodygyroscopejerk.standarddeviation.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>32</td>
<td>average.timebodygyroscopejerk.standarddeviation.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>33</td>
<td>average.timebodyaccelerationmagnitude.mean</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>34</td>
<td>average.timebodyaccelerationmagnitude.standarddeviation</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>35</td>
<td>average.timegravityaccelerationmagnitude.mean</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>36</td>
<td>average.timegravityaccelerationmagnitude.standarddeviation</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>37</td>
<td>average.timebodyaccelerationjerkmagnitude.mean</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>38</td>
<td>average.timebodyaccelerationjerkmagnitude.standarddeviation</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>39</td>
<td>average.timebodygyroscopemagnitude.mean</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>40</td>
<td>average.timebodygyroscopemagnitude.standarddeviation</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>41</td>
<td>average.timebodygyroscopejerkmagnitude.mean</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>42</td>
<td>average.timebodygyroscopejerkmagnitude.standarddeviation</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>43</td>
<td>average.frequencybodyacceleration.mean.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>44</td>
<td>average.frequencybodyacceleration.mean.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>45</td>
<td>average.frequencybodyacceleration.mean.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>46</td>
<td>average.frequencybodyacceleration.standarddeviation.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>47</td>
<td>average.frequencybodyacceleration.standarddeviation.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>48</td>
<td>average.frequencybodyacceleration.standarddeviation.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>49</td>
<td>average.frequencybodyaccelerationjerk.mean.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>50</td>
<td>average.frequencybodyaccelerationjerk.mean.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>51</td>
<td>average.frequencybodyaccelerationjerk.mean.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>52</td>
<td>average.frequencybodyaccelerationjerk.standarddeviation.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>53</td>
<td>average.frequencybodyaccelerationjerk.standarddeviation.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>54</td>
<td>average.frequencybodyaccelerationjerk.standarddeviation.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>55</td>
<td>average.frequencybodygyroscope.mean.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>56</td>
<td>average.frequencybodygyroscope.mean.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>57</td>
<td>average.frequencybodygyroscope.mean.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>58</td>
<td>average.frequencybodygyroscope.standarddeviation.x</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>59</td>
<td>average.frequencybodygyroscope.standarddeviation.y</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>60</td>
<td>average.frequencybodygyroscope.standarddeviation.z</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>61</td>
<td>average.frequencybodyaccelerationmagnitude.mean</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>62</td>
<td>average.frequencybodyaccelerationmagnitude.standarddeviation</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>63</td>
<td>average.frequencybodybodyaccelerationjerkmagnitude.mean</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>64</td>
<td>average.frequencybodybodyaccelerationjerkmagnitude.standarddeviation</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>65</td>
<td>average.frequencybodybodygyroscopemagnitude.mean</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>66</td>
<td>average.frequencybodybodygyroscopemagnitude.standarddeviation</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>67</td>
<td>average.frequencybodybodygyroscopejerkmagnitude.mean</td>
<td>numeric</td>
<td>1</td>
</tr>
<tr>
<td>68</td>
<td>average.frequencybodybodygyroscopejerkmagnitude.standarddeviation</td>
<td>numeric</td>
<td>1</td>
</tr>
</tbody></table>

<h2><a id="user-content-vi-missing-data-code" class="anchor" href="#vi-missing-data-code" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>VI. Missing Data Code</h2>

<p>There exists no missing data.</p>

<h2><a id="user-content-vii-reference" class="anchor" href="#vii-reference" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>VII. Reference</h2>

<p>Anguita, D., Ghio, A., Oneto, L., Parra, X., &amp; Reyes-Ortiz, J. L. (2012). Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine. International Workshop of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. </p>
</article>
  </div>

</div>

<button type="button" data-facebox="#jump-to-line" data-facebox-class="linejump" data-hotkey="l" class="d-none">Jump to Line</button>
<div id="jump-to-line" style="display:none">
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <input class="form-control linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
    <button type="submit" class="btn">Go</button>
</form></div>

  </div>
  <div class="modal-backdrop js-touch-events"></div>
</div>


    </div>
  </div>

    </div>

        <div class="container site-footer-container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links float-right">
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact GitHub</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage" class="site-footer-mark" title="GitHub">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path></svg>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2016 <span title="0.07170s from github-fe-c5e6852.cp1-iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a href="https://help.github.com" data-ga-click="Footer, go to help, text:help">Help</a></li>
    </ul>
  </div>
</div>



    

    <div id="ajax-error-message" class="ajax-error-message flash flash-error">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"></path></svg>
      <button type="button" class="flash-close js-flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
        <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
      </button>
      You can't perform that action at this time.
    </div>


      
      <script crossorigin="anonymous" integrity="sha256-NbnFQdNBMJuTCxx5D6GyejDHxEzhDH+CQokOPYPIrb0=" src="https://assets-cdn.github.com/assets/frameworks-35b9c541d341309b930b1c790fa1b27a30c7c44ce10c7f8242890e3d83c8adbd.js"></script>
      <script async="async" crossorigin="anonymous" integrity="sha256-NjAOUnQ3DcSBV1C8HROMiDYzsEoXXeR3crIdcpaIsIM=" src="https://assets-cdn.github.com/assets/github-36300e5274370dc4815750bc1d138c883633b04a175de47772b21d729688b083.js"></script>
      
      
      
      
    <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner d-none">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"></path></svg>
      <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
      <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
    </div>
    <div class="facebox" id="facebox" style="display:none;">
  <div class="facebox-popup">
    <div class="facebox-content" role="dialog" aria-labelledby="facebox-header" aria-describedby="facebox-description">
    </div>
    <button type="button" class="facebox-close js-facebox-close" aria-label="Close modal">
      <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"></path></svg>
    </button>
  </div>
</div>

  </body>
</html>

