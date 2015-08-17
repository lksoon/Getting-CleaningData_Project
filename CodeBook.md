


<!DOCTYPE html>
<html lang="en" class=" is-copy-enabled">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    <meta name="viewport" content="width=1020">
    
    
    <title>coursera-getting-and-cleaning-data-project/CodeBook.md at master · bgentry/coursera-getting-and-cleaning-data-project</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="bgentry/coursera-getting-and-cleaning-data-project" name="twitter:title" /><meta content="coursera-getting-and-cleaning-data-project - course project for Coursera &quot;Getting and Cleaning Data&quot;" name="twitter:description" /><meta content="https://avatars1.githubusercontent.com/u/114033?v=3&amp;s=400" name="twitter:image:src" />
      <meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars1.githubusercontent.com/u/114033?v=3&amp;s=400" property="og:image" /><meta content="bgentry/coursera-getting-and-cleaning-data-project" property="og:title" /><meta content="https://github.com/bgentry/coursera-getting-and-cleaning-data-project" property="og:url" /><meta content="coursera-getting-and-cleaning-data-project - course project for Coursera &quot;Getting and Cleaning Data&quot;" property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="web-socket" href="wss://live.github.com/_sockets/NjQwNjUwNzphODgyMjA0YWMyNGQyOTVjMjE0MDRlOGI5NWMyZjFmNDoxNDcxYTNmZWIyZWU4ZDNhN2JmYWQ3OGE2OWZmYmNiNDgyYzU0MzQ5OTRlOGU0NjllNGNlNTllZTcyNjIxNTg2--ff0a6237062dc45bfd82bcf857fe5bea21804817">
    <meta name="pjax-timeout" content="1000">
    <link rel="sudo-modal" href="/sessions/sudo_modal">

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>

        <meta name="google-analytics" content="UA-3769691-2">

    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="collector-cdn.github.com" name="octolytics-script-host" /><meta content="github" name="octolytics-app-id" /><meta content="D2BAE7A9:1CB3:4E76912:55D2200A" name="octolytics-dimension-request_id" /><meta content="6406507" name="octolytics-actor-id" /><meta content="lksoon" name="octolytics-actor-login" /><meta content="dd7e9f428a4d7fe4bae3d18a53a8208af2ff027fce842efca88e67787f6eb1a1" name="octolytics-actor-hash" />
    
    <meta content="Rails, view, blob#show" data-pjax-transient="true" name="analytics-event" />
    <meta class="js-ga-set" name="dimension1" content="Logged In">
      <meta class="js-ga-set" name="dimension4" content="Current repo nav">
    <meta name="is-dotcom" content="true">
        <meta name="hostname" content="github.com">
    <meta name="user-login" content="lksoon">

      <link rel="icon" sizes="any" mask href="https://assets-cdn.github.com/pinned-octocat.svg">
      <meta name="theme-color" content="#4078c0">
      <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

    <!-- </textarea> --><!-- '"` --><meta content="authenticity_token" name="csrf-param" />
<meta content="xsR0Al7ms0MRXcSmdfgdQIehJSzMcB/MIrEGmv4pqauDnVs33sYbx6Q5K68KiOAGbbsIKoGmn5Tvul/xBbhWig==" name="csrf-token" />
    <meta content="2bf284fa1f60ba05d088532d588e1822f7724f30" name="form-nonce" />

    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github/index-78350b39bf13714f4b06a2153e5374de01bc939bfa60ec9bdb34dbb2032dda4b.css" media="all" rel="stylesheet" />
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github2/index-fe5622bab39e70fefc28ebe1ea2e8fa620c0c026df4a6b089aac3bf495d3463e.css" media="all" rel="stylesheet" />
    
    


    <meta http-equiv="x-pjax-version" content="a26d7fe411f453e1f88034a366ff5217">

      
  <meta name="description" content="coursera-getting-and-cleaning-data-project - course project for Coursera &quot;Getting and Cleaning Data&quot;">
  <meta name="go-import" content="github.com/bgentry/coursera-getting-and-cleaning-data-project git https://github.com/bgentry/coursera-getting-and-cleaning-data-project.git">

  <meta content="114033" name="octolytics-dimension-user_id" /><meta content="bgentry" name="octolytics-dimension-user_login" /><meta content="32694259" name="octolytics-dimension-repository_id" /><meta content="bgentry/coursera-getting-and-cleaning-data-project" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="32694259" name="octolytics-dimension-repository_network_root_id" /><meta content="bgentry/coursera-getting-and-cleaning-data-project" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/bgentry/coursera-getting-and-cleaning-data-project/commits/master.atom" rel="alternate" title="Recent Commits to coursera-getting-and-cleaning-data-project:master" type="application/atom+xml">

  </head>


  <body class="logged_in  env-production windows vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>
    <div class="wrapper">
      
      
      



        <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" data-ga-click="Header, go to dashboard, icon:logo">
  <span class="mega-octicon octicon-mark-github"></span>
</a>


      <div class="site-search repo-scope js-site-search" role="search">
          <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/bgentry/coursera-getting-and-cleaning-data-project/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/bgentry/coursera-getting-and-cleaning-data-project/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <label class="js-chromeless-input-container form-control">
    <div class="scope-badge">This repository</div>
    <input type="text"
      class="js-site-search-focus js-site-search-field is-clearable chromeless-input"
      data-hotkey="s"
      name="q"
      placeholder="Search"
      aria-label="Search this repository"
      data-global-scope-placeholder="Search GitHub"
      data-repo-scope-placeholder="Search"
      tabindex="1"
      autocapitalize="off">
  </label>
</form>
      </div>

      <ul class="header-nav left" role="navigation">
        <li class="header-nav-item">
          <a href="/pulls" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:pulls context:user" data-hotkey="g p" data-selected-links="/pulls /pulls/assigned /pulls/mentioned /pulls">
            Pull requests
</a>        </li>
        <li class="header-nav-item">
          <a href="/issues" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:issues context:user" data-hotkey="g i" data-selected-links="/issues /issues/assigned /issues/mentioned /issues">
            Issues
</a>        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com/" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
      </ul>

    
<ul class="header-nav user-nav right" id="user-links">
  <li class="header-nav-item">
      <span class="js-socket-channel js-updatable-content"
        data-channel="notification-changed:lksoon"
        data-url="/notifications/header">
      <a href="/notifications" aria-label="You have no unread notifications" class="header-nav-link notification-indicator tooltipped tooltipped-s" data-ga-click="Header, go to notifications, icon:read" data-hotkey="g n">
          <span class="mail-status all-read"></span>
          <span class="octicon octicon-inbox"></span>
</a>  </span>

  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link tooltipped tooltipped-s js-menu-target" href="/new"
       aria-label="Create new…"
       data-ga-click="Header, create new, icon:add">
      <span class="octicon octicon-plus left"></span>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <ul class="dropdown-menu dropdown-menu-sw">
        
<a class="dropdown-item" href="/new" data-ga-click="Header, create new repository">
  New repository
</a>


  <a class="dropdown-item" href="/organizations/new" data-ga-click="Header, create new organization">
    New organization
  </a>



  <div class="dropdown-divider"></div>
  <div class="dropdown-header">
    <span title="bgentry/coursera-getting-and-cleaning-data-project">This repository</span>
  </div>
    <a class="dropdown-item" href="/bgentry/coursera-getting-and-cleaning-data-project/issues/new" data-ga-click="Header, create new issue">
      New issue
    </a>

      </ul>
    </div>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name tooltipped tooltipped-s js-menu-target" href="/lksoon"
       aria-label="View profile and more"
       data-ga-click="Header, show menu, icon:avatar">
      <img alt="@lksoon" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/6406507?v=3&amp;s=40" width="20" />
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <div class="dropdown-menu dropdown-menu-sw">
        <div class="dropdown-header header-nav-current-user css-truncate">
          Signed in as <strong class="css-truncate-target">lksoon</strong>
        </div>
        <div class="dropdown-divider"></div>

        <a class="dropdown-item" href="/lksoon" data-ga-click="Header, go to profile, text:your profile">
          Your profile
        </a>
        <a class="dropdown-item" href="/stars" data-ga-click="Header, go to starred repos, text:your stars">
          Your stars
        </a>
        <a class="dropdown-item" href="/explore" data-ga-click="Header, go to explore, text:explore">
          Explore
        </a>
        <a class="dropdown-item" href="https://help.github.com" data-ga-click="Header, go to help, text:help">
          Help
        </a>
        <div class="dropdown-divider"></div>

        <a class="dropdown-item" href="/settings/profile" data-ga-click="Header, go to settings, icon:settings">
          Settings
        </a>

        <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/logout" class="logout-form" data-form-nonce="2bf284fa1f60ba05d088532d588e1822f7724f30" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="d4l10B8rd1MLkyHpi8BPGVh2EJZVIAHwgvXXt2EDRnOPQozyCqqF3izBRdyQ8iFbuX8e5t1WHmHK4++GrfrOSg==" /></div>
          <button class="dropdown-item dropdown-signout" data-ga-click="Header, sign out, icon:logout">
            Sign out
          </button>
</form>      </div>
    </div>
  </li>
</ul>


    
  </div>
</div>

        

        


      <div id="start-of-content" class="accessibility-aid"></div>
          <div class="site" itemscope itemtype="http://schema.org/WebPage">
    <div id="js-flash-container">
      
    </div>
    <div class="pagehead repohead instapaper_ignore readability-menu ">
      <div class="container">

        <div class="clearfix">
          
<ul class="pagehead-actions">

  <li>
      <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-form-nonce="2bf284fa1f60ba05d088532d588e1822f7724f30" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="VYJepBtCmwNIE8MpjReLr6yfSNvSofcturGyt0DYrUkA307vD8s62vK+RXN19+xCpb9WnP2j5xNLax3CHuemEw==" /></div>    <input id="repository_id" name="repository_id" type="hidden" value="32694259" />

      <div class="select-menu js-menu-container js-select-menu">
        <a href="/bgentry/coursera-getting-and-cleaning-data-project/subscription"
          class="btn btn-sm btn-with-count select-menu-button js-menu-target" role="button" tabindex="0" aria-haspopup="true"
          data-ga-click="Repository, click Watch settings, action:blob#show">
          <span class="js-select-button">
            <span class="octicon octicon-eye"></span>
            Watch
          </span>
        </a>
        <a class="social-count js-social-count" href="/bgentry/coursera-getting-and-cleaning-data-project/watchers">
          0
        </a>

        <div class="select-menu-modal-holder">
          <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
            <div class="select-menu-header">
              <span class="select-menu-title">Notifications</span>
              <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
            </div>

            <div class="select-menu-list js-navigation-container" role="menu">

              <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
                <span class="select-menu-item-icon octicon octicon-check"></span>
                <div class="select-menu-item-text">
                  <input checked="checked" id="do_included" name="do" type="radio" value="included" />
                  <span class="select-menu-item-heading">Not watching</span>
                  <span class="description">Be notified when participating or @mentioned.</span>
                  <span class="js-select-button-text hidden-select-button-text">
                    <span class="octicon octicon-eye"></span>
                    Watch
                  </span>
                </div>
              </div>

              <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                <span class="select-menu-item-icon octicon octicon octicon-check"></span>
                <div class="select-menu-item-text">
                  <input id="do_subscribed" name="do" type="radio" value="subscribed" />
                  <span class="select-menu-item-heading">Watching</span>
                  <span class="description">Be notified of all conversations.</span>
                  <span class="js-select-button-text hidden-select-button-text">
                    <span class="octicon octicon-eye"></span>
                    Unwatch
                  </span>
                </div>
              </div>

              <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                <span class="select-menu-item-icon octicon octicon-check"></span>
                <div class="select-menu-item-text">
                  <input id="do_ignore" name="do" type="radio" value="ignore" />
                  <span class="select-menu-item-heading">Ignoring</span>
                  <span class="description">Never be notified.</span>
                  <span class="js-select-button-text hidden-select-button-text">
                    <span class="octicon octicon-mute"></span>
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

    <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/bgentry/coursera-getting-and-cleaning-data-project/unstar" class="js-toggler-form starred js-unstar-button" data-form-nonce="2bf284fa1f60ba05d088532d588e1822f7724f30" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="P6E4wpncX1iJBoFYowvMRWNJv/adRAa8DeB0TRlliErPal1+/onWnemNXFVWBMa1b9kflElwcoJeyn0v/3R8Rg==" /></div>
      <button
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Unstar this repository" title="Unstar bgentry/coursera-getting-and-cleaning-data-project"
        data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar">
        <span class="octicon octicon-star"></span>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/bgentry/coursera-getting-and-cleaning-data-project/stargazers">
          1
        </a>
</form>
    <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/bgentry/coursera-getting-and-cleaning-data-project/star" class="js-toggler-form unstarred js-star-button" data-form-nonce="2bf284fa1f60ba05d088532d588e1822f7724f30" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="3WhgeEskpBTSDYViq8MQfTMmpzUYIxEzECG3OFbV/ryPi6lgEazdZDROAQJaBxRYgPFN7n8Ozescz5/Axdppew==" /></div>
      <button
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Star this repository" title="Star bgentry/coursera-getting-and-cleaning-data-project"
        data-ga-click="Repository, click star button, action:blob#show; text:Star">
        <span class="octicon octicon-star"></span>
        Star
      </button>
        <a class="social-count js-social-count" href="/bgentry/coursera-getting-and-cleaning-data-project/stargazers">
          1
        </a>
</form>  </div>

  </li>

        <li>
          <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/bgentry/coursera-getting-and-cleaning-data-project/fork" data-form-nonce="2bf284fa1f60ba05d088532d588e1822f7724f30" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="SMtXCXZlz8uGGN+qywcmpdVuYXDbxvHG3Dw8pBTkxa/sc0p3HRqptLZWMXHAwHDkxNHvKHi5ezaYpPNCCIHikw==" /></div>
            <button
                type="submit"
                class="btn btn-sm btn-with-count"
                data-ga-click="Repository, show fork modal, action:blob#show; text:Fork"
                title="Fork your own copy of bgentry/coursera-getting-and-cleaning-data-project to your account"
                aria-label="Fork your own copy of bgentry/coursera-getting-and-cleaning-data-project to your account">
              <span class="octicon octicon-repo-forked"></span>
              Fork
            </button>
            <a href="/bgentry/coursera-getting-and-cleaning-data-project/network" class="social-count">13</a>
</form>        </li>

</ul>

          <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public ">
            <span class="mega-octicon octicon-repo"></span>
            <span class="author"><a href="/bgentry" class="url fn" itemprop="url" rel="author"><span itemprop="title">bgentry</span></a></span><!--
         --><span class="path-divider">/</span><!--
         --><strong><a href="/bgentry/coursera-getting-and-cleaning-data-project" data-pjax="#js-repo-pjax-container">coursera-getting-and-cleaning-data-project</a></strong>

            <span class="page-context-loader">
              <img alt="" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
            </span>

          </h1>
        </div>

      </div>
    </div>

      <div class="container">
        <div class="repository-with-sidebar repo-container new-discussion-timeline ">
          <div class="repository-sidebar clearfix">
              

<nav class="sunken-menu repo-nav js-repo-nav js-sidenav-container-pjax js-octicon-loaders"
     role="navigation"
     data-pjax="#js-repo-pjax-container"
     data-issue-count-url="/bgentry/coursera-getting-and-cleaning-data-project/issues/counts">
  <ul class="sunken-menu-group">
    <li class="tooltipped tooltipped-w" aria-label="Code">
      <a href="/bgentry/coursera-getting-and-cleaning-data-project" aria-label="Code" aria-selected="true" class="js-selected-navigation-item selected sunken-menu-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /bgentry/coursera-getting-and-cleaning-data-project">
        <span class="octicon octicon-code"></span> <span class="full-word">Code</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

      <li class="tooltipped tooltipped-w" aria-label="Issues">
        <a href="/bgentry/coursera-getting-and-cleaning-data-project/issues" aria-label="Issues" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /bgentry/coursera-getting-and-cleaning-data-project/issues">
          <span class="octicon octicon-issue-opened"></span> <span class="full-word">Issues</span>
          <span class="js-issue-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>

    <li class="tooltipped tooltipped-w" aria-label="Pull requests">
      <a href="/bgentry/coursera-getting-and-cleaning-data-project/pulls" aria-label="Pull requests" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g p" data-selected-links="repo_pulls /bgentry/coursera-getting-and-cleaning-data-project/pulls">
          <span class="octicon octicon-git-pull-request"></span> <span class="full-word">Pull requests</span>
          <span class="js-pull-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

      <li class="tooltipped tooltipped-w" aria-label="Wiki">
        <a href="/bgentry/coursera-getting-and-cleaning-data-project/wiki" aria-label="Wiki" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g w" data-selected-links="repo_wiki /bgentry/coursera-getting-and-cleaning-data-project/wiki">
          <span class="octicon octicon-book"></span> <span class="full-word">Wiki</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>
  </ul>
  <div class="sunken-menu-separator"></div>
  <ul class="sunken-menu-group">

    <li class="tooltipped tooltipped-w" aria-label="Pulse">
      <a href="/bgentry/coursera-getting-and-cleaning-data-project/pulse" aria-label="Pulse" class="js-selected-navigation-item sunken-menu-item" data-selected-links="pulse /bgentry/coursera-getting-and-cleaning-data-project/pulse">
        <span class="octicon octicon-pulse"></span> <span class="full-word">Pulse</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

    <li class="tooltipped tooltipped-w" aria-label="Graphs">
      <a href="/bgentry/coursera-getting-and-cleaning-data-project/graphs" aria-label="Graphs" class="js-selected-navigation-item sunken-menu-item" data-selected-links="repo_graphs repo_contributors /bgentry/coursera-getting-and-cleaning-data-project/graphs">
        <span class="octicon octicon-graph"></span> <span class="full-word">Graphs</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>
  </ul>


</nav>

                <div class="only-with-full-nav">
                    
<div class="js-clone-url clone-url open"
  data-protocol-type="http">
  <h3><span class="text-emphasized">HTTPS</span> clone URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/bgentry/coursera-getting-and-cleaning-data-project.git" readonly="readonly" aria-label="HTTPS clone URL">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="js-clone-url clone-url "
  data-protocol-type="ssh">
  <h3><span class="text-emphasized">SSH</span> clone URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="git@github.com:bgentry/coursera-getting-and-cleaning-data-project.git" readonly="readonly" aria-label="SSH clone URL">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="js-clone-url clone-url "
  data-protocol-type="subversion">
  <h3><span class="text-emphasized">Subversion</span> checkout URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/bgentry/coursera-getting-and-cleaning-data-project" readonly="readonly" aria-label="Subversion checkout URL">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>



  <div class="clone-options">You can clone with
    <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/users/set_protocol?protocol_selector=http&amp;protocol_type=clone" class="inline-form js-clone-selector-form is-enabled" data-form-nonce="2bf284fa1f60ba05d088532d588e1822f7724f30" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="qOPJ5Pxn4Z+Bu65WZdX2WrFBhl2Kdt6PBbjGwnHciHxNF63Rak3ustcd0pZ55wsw1gtoOMCvGsi+gGIchivJXw==" /></div><button class="btn-link js-clone-selector" data-protocol="http" type="submit">HTTPS</button></form>, <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/users/set_protocol?protocol_selector=ssh&amp;protocol_type=clone" class="inline-form js-clone-selector-form is-enabled" data-form-nonce="2bf284fa1f60ba05d088532d588e1822f7724f30" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="rHCS79s67V1lOnZM1+xSnRw2lwuPLjLqmREhJRJCZmXFjRXTXoPF62e3/PbpFutCaH9UfxpnREjAuw8/DQ11TQ==" /></div><button class="btn-link js-clone-selector" data-protocol="ssh" type="submit">SSH</button></form>, or <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/users/set_protocol?protocol_selector=subversion&amp;protocol_type=clone" class="inline-form js-clone-selector-form is-enabled" data-form-nonce="2bf284fa1f60ba05d088532d588e1822f7724f30" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="s0ai16x3vFSMh/fwdm+6S79arul/RlMfndk0gApm0o++Ay1L+Lz4PuKzdK6ckf+ok48qhs/xdjKoidaVTxrUzA==" /></div><button class="btn-link js-clone-selector" data-protocol="subversion" type="submit">Subversion</button></form>.
    <a href="https://help.github.com/articles/which-remote-url-should-i-use" class="help tooltipped tooltipped-n" aria-label="Get help on which URL is right for you.">
      <span class="octicon octicon-question"></span>
    </a>
  </div>
    <a href="github-windows://openRepo/https://github.com/bgentry/coursera-getting-and-cleaning-data-project" class="btn btn-sm sidebar-button" title="Save bgentry/coursera-getting-and-cleaning-data-project to your computer and use it in GitHub Desktop." aria-label="Save bgentry/coursera-getting-and-cleaning-data-project to your computer and use it in GitHub Desktop.">
      <span class="octicon octicon-desktop-download"></span>
      Clone in Desktop
    </a>

                  <a href="/bgentry/coursera-getting-and-cleaning-data-project/archive/master.zip"
                     class="btn btn-sm sidebar-button"
                     aria-label="Download the contents of bgentry/coursera-getting-and-cleaning-data-project as a zip file"
                     title="Download the contents of bgentry/coursera-getting-and-cleaning-data-project as a zip file"
                     rel="nofollow">
                    <span class="octicon octicon-cloud-download"></span>
                    Download ZIP
                  </a>
                </div>
          </div>
          <div id="js-repo-pjax-container" class="repository-content context-loader-container" data-pjax-container>

            

<a href="/bgentry/coursera-getting-and-cleaning-data-project/blob/f970ecbd764eaec92c220d8b28c55b44941fa2a6/CodeBook.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:4d305355484bf387e1741d86271d912f -->

  <div class="file-navigation js-zeroclipboard-container">
    
<div class="select-menu js-menu-container js-select-menu left">
  <span class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    data-ref="master"
    title="master"
    role="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <i>Branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </span>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <span class="select-menu-title">Switch branches/tags</span>
        <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
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
               href="/bgentry/coursera-getting-and-cleaning-data-project/blob/master/CodeBook.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <span class="select-menu-item-text css-truncate-target" title="master">
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

    <div class="btn-group right">
      <a href="/bgentry/coursera-getting-and-cleaning-data-project/find/master"
            class="js-show-file-finder btn btn-sm empty-icon tooltipped tooltipped-nw"
            data-pjax
            data-hotkey="t"
            aria-label="Quickly jump between files">
        <span class="octicon octicon-list-unordered"></span>
      </a>
      <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </div>

    <div class="breadcrumb js-zeroclipboard-target">
      <span class="repo-root js-repo-root"><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/bgentry/coursera-getting-and-cleaning-data-project" class="" data-branch="master" data-pjax="true" itemscope="url"><span itemprop="title">coursera-getting-and-cleaning-data-project</span></a></span></span><span class="separator">/</span><strong class="final-path">CodeBook.md</strong>
    </div>
  </div>


  <div class="commit file-history-tease">
    <div class="file-history-tease-header">
        <img alt="@bgentry" class="avatar" height="24" src="https://avatars0.githubusercontent.com/u/114033?v=3&amp;s=48" width="24" />
        <span class="author"><a href="/bgentry" rel="author">bgentry</a></span>
        <time datetime="2015-03-22T20:36:43Z" is="relative-time">Mar 22, 2015</time>
        <div class="commit-title">
            <a href="/bgentry/coursera-getting-and-cleaning-data-project/commit/f970ecbd764eaec92c220d8b28c55b44941fa2a6" class="message" data-pjax="true" title="add code book">add code book</a>
        </div>
    </div>

    <div class="participation">
      <p class="quickstat">
        <a href="#blob_contributors_box" rel="facebox">
          <strong>1</strong>
           contributor
        </a>
      </p>
      
    </div>
    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list">
          <li class="facebox-user-list-item">
            <img alt="@bgentry" height="24" src="https://avatars0.githubusercontent.com/u/114033?v=3&amp;s=48" width="24" />
            <a href="/bgentry">bgentry</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file">
  <div class="file-header">
    <div class="file-actions">

      <div class="btn-group">
        <a href="/bgentry/coursera-getting-and-cleaning-data-project/raw/master/CodeBook.md" class="btn btn-sm " id="raw-url">Raw</a>
          <a href="/bgentry/coursera-getting-and-cleaning-data-project/blame/master/CodeBook.md" class="btn btn-sm js-update-url-with-hash">Blame</a>
        <a href="/bgentry/coursera-getting-and-cleaning-data-project/commits/master/CodeBook.md" class="btn btn-sm " rel="nofollow">History</a>
      </div>

        <a class="octicon-btn tooltipped tooltipped-nw"
           href="github-windows://openRepo/https://github.com/bgentry/coursera-getting-and-cleaning-data-project?branch=master&amp;filepath=CodeBook.md"
           aria-label="Open this file in GitHub Desktop"
           data-ga-click="Repository, open with desktop, type:windows">
            <span class="octicon octicon-desktop-download"></span>
        </a>

            <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/bgentry/coursera-getting-and-cleaning-data-project/edit/master/CodeBook.md" class="inline-form" data-form-nonce="2bf284fa1f60ba05d088532d588e1822f7724f30" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="K4KWVPPcipmyVK3KZIR3ipstvatm3X+6EkKSWP2SRx8rwcTEke3EP/eEXmLVQvDCibr3noTl7EyCOY2bHYWTbQ==" /></div>
              <button class="octicon-btn tooltipped tooltipped-n" type="submit" aria-label="Fork this project and edit the file" data-hotkey="e" data-disable-with>
                <span class="octicon octicon-pencil"></span>
              </button>
</form>
          <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/bgentry/coursera-getting-and-cleaning-data-project/delete/master/CodeBook.md" class="inline-form" data-form-nonce="2bf284fa1f60ba05d088532d588e1822f7724f30" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="i1+vHWTZqXLqVeuR9nZsqEIYcqRsfwavytjeMPG8zqKjBLWl5AExDw5lL5/TXL4viuighbaxMTZI29i1FrNqgQ==" /></div>
            <button class="octicon-btn octicon-btn-danger tooltipped tooltipped-n" type="submit" aria-label="Fork this project and delete this file" data-disable-with>
              <span class="octicon octicon-trashcan"></span>
            </button>
</form>    </div>

    <div class="file-info">
        100 lines (92 sloc)
        <span class="file-info-divider"></span>
      2.393 kB
    </div>
  </div>
  
  <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1><a id="user-content-code-book" class="anchor" href="#code-book" aria-hidden="true"><span class="octicon octicon-link"></span></a>Code Book</h1>

<p>This code book summarizes the resulting data fields in <code>tidy.txt</code>.</p>

<h2><a id="user-content-identifiers" class="anchor" href="#identifiers" aria-hidden="true"><span class="octicon octicon-link"></span></a>Identifiers</h2>

<ul>
<li><code>subject</code> - The ID of the test subject</li>
<li><code>activity</code> - The type of activity performed when the corresponding measurements were taken</li>
</ul>

<h2><a id="user-content-measurements" class="anchor" href="#measurements" aria-hidden="true"><span class="octicon octicon-link"></span></a>Measurements</h2>

<ul>
<li><code>tBodyAccMeanX</code></li>
<li><code>tBodyAccMeanY</code></li>
<li><code>tBodyAccMeanZ</code></li>
<li><code>tBodyAccStdX</code></li>
<li><code>tBodyAccStdY</code></li>
<li><code>tBodyAccStdZ</code></li>
<li><code>tGravityAccMeanX</code></li>
<li><code>tGravityAccMeanY</code></li>
<li><code>tGravityAccMeanZ</code></li>
<li><code>tGravityAccStdX</code></li>
<li><code>tGravityAccStdY</code></li>
<li><code>tGravityAccStdZ</code></li>
<li><code>tBodyAccJerkMeanX</code></li>
<li><code>tBodyAccJerkMeanY</code></li>
<li><code>tBodyAccJerkMeanZ</code></li>
<li><code>tBodyAccJerkStdX</code></li>
<li><code>tBodyAccJerkStdY</code></li>
<li><code>tBodyAccJerkStdZ</code></li>
<li><code>tBodyGyroMeanX</code></li>
<li><code>tBodyGyroMeanY</code></li>
<li><code>tBodyGyroMeanZ</code></li>
<li><code>tBodyGyroStdX</code></li>
<li><code>tBodyGyroStdY</code></li>
<li><code>tBodyGyroStdZ</code></li>
<li><code>tBodyGyroJerkMeanX</code></li>
<li><code>tBodyGyroJerkMeanY</code></li>
<li><code>tBodyGyroJerkMeanZ</code></li>
<li><code>tBodyGyroJerkStdX</code></li>
<li><code>tBodyGyroJerkStdY</code></li>
<li><code>tBodyGyroJerkStdZ</code></li>
<li><code>tBodyAccMagMean</code></li>
<li><code>tBodyAccMagStd</code></li>
<li><code>tGravityAccMagMean</code></li>
<li><code>tGravityAccMagStd</code></li>
<li><code>tBodyAccJerkMagMean</code></li>
<li><code>tBodyAccJerkMagStd</code></li>
<li><code>tBodyGyroMagMean</code></li>
<li><code>tBodyGyroMagStd</code></li>
<li><code>tBodyGyroJerkMagMean</code></li>
<li><code>tBodyGyroJerkMagStd</code></li>
<li><code>fBodyAccMeanX</code></li>
<li><code>fBodyAccMeanY</code></li>
<li><code>fBodyAccMeanZ</code></li>
<li><code>fBodyAccStdX</code></li>
<li><code>fBodyAccStdY</code></li>
<li><code>fBodyAccStdZ</code></li>
<li><code>fBodyAccMeanFreqX</code></li>
<li><code>fBodyAccMeanFreqY</code></li>
<li><code>fBodyAccMeanFreqZ</code></li>
<li><code>fBodyAccJerkMeanX</code></li>
<li><code>fBodyAccJerkMeanY</code></li>
<li><code>fBodyAccJerkMeanZ</code></li>
<li><code>fBodyAccJerkStdX</code></li>
<li><code>fBodyAccJerkStdY</code></li>
<li><code>fBodyAccJerkStdZ</code></li>
<li><code>fBodyAccJerkMeanFreqX</code></li>
<li><code>fBodyAccJerkMeanFreqY</code></li>
<li><code>fBodyAccJerkMeanFreqZ</code></li>
<li><code>fBodyGyroMeanX</code></li>
<li><code>fBodyGyroMeanY</code></li>
<li><code>fBodyGyroMeanZ</code></li>
<li><code>fBodyGyroStdX</code></li>
<li><code>fBodyGyroStdY</code></li>
<li><code>fBodyGyroStdZ</code></li>
<li><code>fBodyGyroMeanFreqX</code></li>
<li><code>fBodyGyroMeanFreqY</code></li>
<li><code>fBodyGyroMeanFreqZ</code></li>
<li><code>fBodyAccMagMean</code></li>
<li><code>fBodyAccMagStd</code></li>
<li><code>fBodyAccMagMeanFreq</code></li>
<li><code>fBodyBodyAccJerkMagMean</code></li>
<li><code>fBodyBodyAccJerkMagStd</code></li>
<li><code>fBodyBodyAccJerkMagMeanFreq</code></li>
<li><code>fBodyBodyGyroMagMean</code></li>
<li><code>fBodyBodyGyroMagStd</code></li>
<li><code>fBodyBodyGyroMagMeanFreq</code></li>
<li><code>fBodyBodyGyroJerkMagMean</code></li>
<li><code>fBodyBodyGyroJerkMagStd</code></li>
<li><code>fBodyBodyGyroJerkMagMeanFreq</code></li>
</ul>

<h2><a id="user-content-activity-labels" class="anchor" href="#activity-labels" aria-hidden="true"><span class="octicon octicon-link"></span></a>Activity Labels</h2>

<ul>
<li><code>WALKING</code> (value <code>1</code>): subject was walking during the test</li>
<li><code>WALKING_UPSTAIRS</code> (value <code>2</code>): subject was walking up a staircase during the test</li>
<li><code>WALKING_DOWNSTAIRS</code> (value <code>3</code>): subject was walking down a staircase during the test</li>
<li><code>SITTING</code> (value <code>4</code>): subject was sitting during the test</li>
<li><code>STANDING</code> (value <code>5</code>): subject was standing during the test</li>
<li><code>LAYING</code> (value <code>6</code>): subject was laying down during the test</li>
</ul>
</article>
  </div>

</div>

<a href="#jump-to-line" rel="facebox[.linejump]" data-hotkey="l" style="display:none">Jump to Line</a>
<div id="jump-to-line" style="display:none">
  <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
    <button type="submit" class="btn">Go</button>
</form></div>

          </div>
        </div>
        <div class="modal-backdrop"></div>
      </div>
  </div>


    </div><!-- /.wrapper -->

      <div class="container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links right">
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>
        <li><a href="https://help.github.com" data-ga-click="Footer, go to help, text:help">Help</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage">
      <span class="mega-octicon octicon-mark-github" title="GitHub"></span>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2015 <span title="0.07989s from github-fe120-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact</a></li>
    </ul>
  </div>
</div>


    <div class="fullscreen-overlay js-fullscreen-overlay" id="fullscreen_overlay">
  <div class="fullscreen-container js-suggester-container">
    <div class="textarea-wrap">
      <textarea name="fullscreen-contents" id="fullscreen-contents" class="fullscreen-contents js-fullscreen-contents" placeholder="" aria-label=""></textarea>
      <div class="suggester-container">
        <div class="suggester fullscreen-suggester js-suggester js-navigation-container"></div>
      </div>
    </div>
  </div>
  <div class="fullscreen-sidebar">
    <a href="#" class="exit-fullscreen js-exit-fullscreen tooltipped tooltipped-w" aria-label="Exit Zen Mode">
      <span class="mega-octicon octicon-screen-normal"></span>
    </a>
    <a href="#" class="theme-switcher js-theme-switcher tooltipped tooltipped-w"
      aria-label="Switch themes">
      <span class="octicon octicon-color-mode"></span>
    </a>
  </div>
</div>



    
    

    <div id="ajax-error-message" class="flash flash-error">
      <span class="octicon octicon-alert"></span>
      <a href="#" class="octicon octicon-x flash-close js-ajax-error-dismiss" aria-label="Dismiss error"></a>
      Something went wrong with that request. Please try again.
    </div>


      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-55bdb89972afd4b256fc7c3ed42001976a03fb3eaba96e625d5806c659bc19c6.js"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github/index-fe2e1fa6704baa94c97c39847254262f674803845a2b1addd89d4f9eca3fa297.js"></script>
      
      
    <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner hidden">
      <span class="octicon octicon-alert"></span>
      <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
      <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
    </div>
  </body>
</html>

