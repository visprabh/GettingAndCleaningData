



<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    
    
    <title>GettingAndCleaningData/CodeBook.md at master · ntnmathur/GettingAndCleaningData</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="ntnmathur/GettingAndCleaningData" name="twitter:title" /><meta content="Contribute to GettingAndCleaningData development by creating an account on GitHub." name="twitter:description" /><meta content="https://avatars3.githubusercontent.com/u/7801923?v=2&amp;s=400" name="twitter:image:src" />
<meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars3.githubusercontent.com/u/7801923?v=2&amp;s=400" property="og:image" /><meta content="ntnmathur/GettingAndCleaningData" property="og:title" /><meta content="https://github.com/ntnmathur/GettingAndCleaningData" property="og:url" /><meta content="Contribute to GettingAndCleaningData development by creating an account on GitHub." property="og:description" />

      <meta name="browser-stats-url" content="/_stats">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="conduit-xhr" href="https://ghconduit.com:25035">
    <link rel="xhr-socket" href="/_sockets">

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>
      <meta name="google-analytics" content="UA-3769691-2">

    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="collector-cdn.github.com" name="octolytics-script-host" /><meta content="github" name="octolytics-app-id" /><meta content="1806B3BE:5B17:15A7FF65:541F61D3" name="octolytics-dimension-request_id" /><meta content="8162945" name="octolytics-actor-id" /><meta content="visprabh" name="octolytics-actor-login" /><meta content="ca9867aa7838413f1a9cc3c37c1d324143077d988af7252525243c0e2f52bc0f" name="octolytics-actor-hash" />
    <meta content="Rails, view, blob#show" name="analytics-event" />

    
    
    <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">


    <meta content="authenticity_token" name="csrf-param" />
<meta content="47OyRDbr5TgIIvN9ArxPoUz4ateG3dGLwwMkIlpxVgQQsdnVPZQSv5Q4+Wto9pZh0FQPTN59xTbFtAODMjHuIg==" name="csrf-token" />

    <link href="https://assets-cdn.github.com/assets/github-b83b8eb08bbe9393c7a5d777e6a86ffe4372ab2d.css" media="all" rel="stylesheet" type="text/css" />
    <link href="https://assets-cdn.github.com/assets/github2-6974f31de378b725bc92bba2de583f0def78777d.css" media="all" rel="stylesheet" type="text/css" />
    


    <meta http-equiv="x-pjax-version" content="e8f7e8a0a03c89ddad1f42c7a22f1828">

      
  <meta name="description" content="Contribute to GettingAndCleaningData development by creating an account on GitHub.">
  <meta name="go-import" content="github.com/ntnmathur/GettingAndCleaningData git https://github.com/ntnmathur/GettingAndCleaningData.git">

  <meta content="7801923" name="octolytics-dimension-user_id" /><meta content="ntnmathur" name="octolytics-dimension-user_login" /><meta content="24307032" name="octolytics-dimension-repository_id" /><meta content="ntnmathur/GettingAndCleaningData" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="24307032" name="octolytics-dimension-repository_network_root_id" /><meta content="ntnmathur/GettingAndCleaningData" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/ntnmathur/GettingAndCleaningData/commits/master.atom" rel="alternate" title="Recent Commits to GettingAndCleaningData:master" type="application/atom+xml">

  </head>


  <body class="logged_in  env-production macintosh vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>
    <div class="wrapper">
      
      
      
      


      <div class="header header-logged-in true">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" aria-label="Homepage" ga-data-click="Header, go to dashboard, icon:logo">
  <span class="mega-octicon octicon-mark-github"></span>
</a>


      <div class="site-search repo-scope js-site-search">
          <form accept-charset="UTF-8" action="/ntnmathur/GettingAndCleaningData/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/ntnmathur/GettingAndCleaningData/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <input type="text"
    class="js-site-search-field is-clearable"
    data-hotkey="s"
    name="q"
    placeholder="Search"
    data-global-scope-placeholder="Search GitHub"
    data-repo-scope-placeholder="Search"
    tabindex="1"
    autocapitalize="off">
  <div class="scope-badge">This repository</div>
</form>
      </div>
      <ul class="header-nav left">
        <li class="header-nav-item explore">
          <a class="header-nav-link" href="/explore" data-ga-click="Header, go to explore, text:explore">Explore</a>
        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/blog" data-ga-click="Header, go to blog, text:blog">Blog</a>
          </li>
        <li class="header-nav-item">
          <a class="header-nav-link" href="https://help.github.com" data-ga-click="Header, go to help, text:help">Help</a>
        </li>
      </ul>

    
<ul class="header-nav user-nav right" id="user-links">
  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name" href="/visprabh" data-ga-click="Header, go to profile, text:username">
      <img alt="Vishnu Prabhakar" class="avatar" data-user="8162945" height="20" src="https://avatars3.githubusercontent.com/u/8162945?v=2&amp;s=40" width="20" />
      <span class="css-truncate">
        <span class="css-truncate-target">visprabh</span>
      </span>
    </a>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link js-menu-target tooltipped tooltipped-s" href="#" aria-label="Create new..." data-ga-click="Header, create new, icon:add">
      <span class="octicon octicon-plus"></span>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      
<ul class="dropdown-menu">
  <li>
    <a href="/new"><span class="octicon octicon-repo"></span> New repository</a>
  </li>
  <li>
    <a href="/organizations/new"><span class="octicon octicon-organization"></span> New organization</a>
  </li>


    <li class="dropdown-divider"></li>
    <li class="dropdown-header">
      <span title="ntnmathur/GettingAndCleaningData">This repository</span>
    </li>
      <li>
        <a href="/ntnmathur/GettingAndCleaningData/issues/new"><span class="octicon octicon-issue-opened"></span> New issue</a>
      </li>
</ul>

    </div>
  </li>

  <li class="header-nav-item">
        <a href="/notifications" aria-label="You have no unread notifications" class="header-nav-link notification-indicator tooltipped tooltipped-s" data-ga-click="Header, go to notifications, icon:read" data-hotkey="g n">
        <span class="mail-status all-read"></span>
        <span class="octicon octicon-inbox"></span>
</a>
  </li>

  <li class="header-nav-item">
    <a class="header-nav-link tooltipped tooltipped-s" href="/settings/profile" id="account_settings" aria-label="Settings" data-ga-click="Header, go to settings, icon:settings">
      <span class="octicon octicon-gear"></span>
    </a>
  </li>

  <li class="header-nav-item">
    <form accept-charset="UTF-8" action="/logout" class="logout-form" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="3dFxFSpVjaWPzpz5CkgAp0ar6rdBNj3z8WpHgzQuJ8PSCULTD6kuYnsZZIH7hfF6cpSTJYCXUrlpKWlQhN3XyA==" /></div>
      <button class="header-nav-link sign-out-button tooltipped tooltipped-s" aria-label="Sign out" data-ga-click="Header, sign out, icon:logout">
        <span class="octicon octicon-sign-out"></span>
      </button>
</form>  </li>

</ul>


    
  </div>
</div>

      

        


      <div id="start-of-content" class="accessibility-aid"></div>
          <div class="site" itemscope itemtype="http://schema.org/WebPage">
    <div id="js-flash-container">
      
    </div>
    <div class="pagehead repohead instapaper_ignore readability-menu">
      <div class="container">
        
<ul class="pagehead-actions">

    <li class="subscription">
      <form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="E6rF1VRQwbfo73ILguUU69iHZQTUpyLeiUU0AAuySIar/K7NX7upwRDbknhTVJ0PYznpTEG+rUz9gq+jJ9AlVQ==" /></div>  <input id="repository_id" name="repository_id" type="hidden" value="24307032" />

    <div class="select-menu js-menu-container js-select-menu">
      <a class="social-count js-social-count" href="/ntnmathur/GettingAndCleaningData/watchers">
        1
      </a>
      <a href="/ntnmathur/GettingAndCleaningData/subscription"
        class="minibutton select-menu-button with-count js-menu-target" role="button" tabindex="0" aria-haspopup="true">
        <span class="js-select-button">
          <span class="octicon octicon-eye"></span>
          Watch
        </span>
      </a>

      <div class="select-menu-modal-holder">
        <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
          <div class="select-menu-header">
            <span class="select-menu-title">Notifications</span>
            <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
          </div> <!-- /.select-menu-header -->

          <div class="select-menu-list js-navigation-container" role="menu">

            <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input checked="checked" id="do_included" name="do" type="radio" value="included" />
                <h4>Not watching</h4>
                <span class="description">Be notified when participating or @mentioned.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-eye"></span>
                  Watch
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

            <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input id="do_subscribed" name="do" type="radio" value="subscribed" />
                <h4>Watching</h4>
                <span class="description">Be notified of all conversations.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-eye"></span>
                  Unwatch
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

            <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input id="do_ignore" name="do" type="radio" value="ignore" />
                <h4>Ignoring</h4>
                <span class="description">Never be notified.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-mute"></span>
                  Stop ignoring
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

          </div> <!-- /.select-menu-list -->

        </div> <!-- /.select-menu-modal -->
      </div> <!-- /.select-menu-modal-holder -->
    </div> <!-- /.select-menu -->

</form>
    </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <form accept-charset="UTF-8" action="/ntnmathur/GettingAndCleaningData/unstar" class="js-toggler-form starred js-unstar-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="PXqf1DBR5M3YiK1U+pMhjxFqJz2w1suZi2Ez/oAl/VEMRmfiWmZhujVC0TX+WUt6fpRf6cl6p0oXzAUbDUq+pA==" /></div>
      <button
        class="minibutton with-count js-toggler-target star-button"
        aria-label="Unstar this repository" title="Unstar ntnmathur/GettingAndCleaningData">
        <span class="octicon octicon-star"></span>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/ntnmathur/GettingAndCleaningData/stargazers">
          0
        </a>
</form>
    <form accept-charset="UTF-8" action="/ntnmathur/GettingAndCleaningData/star" class="js-toggler-form unstarred js-star-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="g4D0dWAkBCZ9QBx5uFWIQPp9W24ouequZAljgVkWA+KyCkPHMdWzObvBW3ch1emgF6b+7syc23xaZZn4GKWy7g==" /></div>
      <button
        class="minibutton with-count js-toggler-target star-button"
        aria-label="Star this repository" title="Star ntnmathur/GettingAndCleaningData">
        <span class="octicon octicon-star"></span>
        Star
      </button>
        <a class="social-count js-social-count" href="/ntnmathur/GettingAndCleaningData/stargazers">
          0
        </a>
</form>  </div>

  </li>


        <li>
          <a href="/ntnmathur/GettingAndCleaningData/fork" class="minibutton with-count js-toggler-target fork-button tooltipped-n" title="Fork your own copy of ntnmathur/GettingAndCleaningData to your account" aria-label="Fork your own copy of ntnmathur/GettingAndCleaningData to your account" rel="nofollow" data-method="post">
            <span class="octicon octicon-repo-forked"></span>
            Fork
          </a>
          <a href="/ntnmathur/GettingAndCleaningData/network" class="social-count">0</a>
        </li>

</ul>

        <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public">
          <span class="mega-octicon octicon-repo"></span>
          <span class="author"><a href="/ntnmathur" class="url fn" itemprop="url" rel="author"><span itemprop="title">ntnmathur</span></a></span><!--
       --><span class="path-divider">/</span><!--
       --><strong><a href="/ntnmathur/GettingAndCleaningData" class="js-current-repository js-repo-home-link">GettingAndCleaningData</a></strong>

          <span class="page-context-loader">
            <img alt="" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
          </span>

        </h1>
      </div><!-- /.container -->
    </div><!-- /.repohead -->

    <div class="container">
      <div class="repository-with-sidebar repo-container new-discussion-timeline  ">
        <div class="repository-sidebar clearfix">
            
<div class="sunken-menu vertical-right repo-nav js-repo-nav js-repository-container-pjax js-octicon-loaders" data-issue-count-url="/ntnmathur/GettingAndCleaningData/issues/counts">
  <div class="sunken-menu-contents">
    <ul class="sunken-menu-group">
      <li class="tooltipped tooltipped-w" aria-label="Code">
        <a href="/ntnmathur/GettingAndCleaningData" aria-label="Code" class="selected js-selected-navigation-item sunken-menu-item" data-hotkey="g c" data-pjax="true" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /ntnmathur/GettingAndCleaningData">
          <span class="octicon octicon-code"></span> <span class="full-word">Code</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>

        <li class="tooltipped tooltipped-w" aria-label="Issues">
          <a href="/ntnmathur/GettingAndCleaningData/issues" aria-label="Issues" class="js-selected-navigation-item sunken-menu-item js-disable-pjax" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /ntnmathur/GettingAndCleaningData/issues">
            <span class="octicon octicon-issue-opened"></span> <span class="full-word">Issues</span>
            <span class="js-issue-replace-counter"></span>
            <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>        </li>

      <li class="tooltipped tooltipped-w" aria-label="Pull Requests">
        <a href="/ntnmathur/GettingAndCleaningData/pulls" aria-label="Pull Requests" class="js-selected-navigation-item sunken-menu-item js-disable-pjax" data-hotkey="g p" data-selected-links="repo_pulls /ntnmathur/GettingAndCleaningData/pulls">
            <span class="octicon octicon-git-pull-request"></span> <span class="full-word">Pull Requests</span>
            <span class="js-pull-replace-counter"></span>
            <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>


        <li class="tooltipped tooltipped-w" aria-label="Wiki">
          <a href="/ntnmathur/GettingAndCleaningData/wiki" aria-label="Wiki" class="js-selected-navigation-item sunken-menu-item js-disable-pjax" data-hotkey="g w" data-selected-links="repo_wiki /ntnmathur/GettingAndCleaningData/wiki">
            <span class="octicon octicon-book"></span> <span class="full-word">Wiki</span>
            <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>        </li>
    </ul>
    <div class="sunken-menu-separator"></div>
    <ul class="sunken-menu-group">

      <li class="tooltipped tooltipped-w" aria-label="Pulse">
        <a href="/ntnmathur/GettingAndCleaningData/pulse/weekly" aria-label="Pulse" class="js-selected-navigation-item sunken-menu-item" data-pjax="true" data-selected-links="pulse /ntnmathur/GettingAndCleaningData/pulse/weekly">
          <span class="octicon octicon-pulse"></span> <span class="full-word">Pulse</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>

      <li class="tooltipped tooltipped-w" aria-label="Graphs">
        <a href="/ntnmathur/GettingAndCleaningData/graphs" aria-label="Graphs" class="js-selected-navigation-item sunken-menu-item" data-pjax="true" data-selected-links="repo_graphs repo_contributors /ntnmathur/GettingAndCleaningData/graphs">
          <span class="octicon octicon-graph"></span> <span class="full-word">Graphs</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>
    </ul>


  </div>
</div>

              <div class="only-with-full-nav">
                
  
<div class="clone-url open"
  data-protocol-type="http"
  data-url="/users/set_protocol?protocol_selector=http&amp;protocol_type=clone">
  <h3><span class="text-emphasized">HTTPS</span> clone URL</h3>
  <div class="input-group">
    <input type="text" class="input-mini input-monospace js-url-field"
           value="https://github.com/ntnmathur/GettingAndCleaningData.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-clipboard-text="https://github.com/ntnmathur/GettingAndCleaningData.git" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="ssh"
  data-url="/users/set_protocol?protocol_selector=ssh&amp;protocol_type=clone">
  <h3><span class="text-emphasized">SSH</span> clone URL</h3>
  <div class="input-group">
    <input type="text" class="input-mini input-monospace js-url-field"
           value="git@github.com:ntnmathur/GettingAndCleaningData.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-clipboard-text="git@github.com:ntnmathur/GettingAndCleaningData.git" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="subversion"
  data-url="/users/set_protocol?protocol_selector=subversion&amp;protocol_type=clone">
  <h3><span class="text-emphasized">Subversion</span> checkout URL</h3>
  <div class="input-group">
    <input type="text" class="input-mini input-monospace js-url-field"
           value="https://github.com/ntnmathur/GettingAndCleaningData" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-clipboard-text="https://github.com/ntnmathur/GettingAndCleaningData" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>


<p class="clone-options">You can clone with
      <a href="#" class="js-clone-selector" data-protocol="http">HTTPS</a>,
      <a href="#" class="js-clone-selector" data-protocol="ssh">SSH</a>,
      or <a href="#" class="js-clone-selector" data-protocol="subversion">Subversion</a>.
  <a href="https://help.github.com/articles/which-remote-url-should-i-use" class="help tooltipped tooltipped-n" aria-label="Get help on which URL is right for you.">
    <span class="octicon octicon-question"></span>
  </a>
</p>

  <a href="http://mac.github.com" data-url="github-mac://openRepo/https://github.com/ntnmathur/GettingAndCleaningData" class="minibutton sidebar-button js-conduit-rewrite-url" title="Save ntnmathur/GettingAndCleaningData to your computer and use it in GitHub Desktop." aria-label="Save ntnmathur/GettingAndCleaningData to your computer and use it in GitHub Desktop.">
    <span class="octicon octicon-device-desktop"></span>
    Clone in Desktop
  </a>


                <a href="/ntnmathur/GettingAndCleaningData/archive/master.zip"
                   class="minibutton sidebar-button"
                   aria-label="Download the contents of ntnmathur/GettingAndCleaningData as a zip file"
                   title="Download the contents of ntnmathur/GettingAndCleaningData as a zip file"
                   rel="nofollow">
                  <span class="octicon octicon-cloud-download"></span>
                  Download ZIP
                </a>
              </div>
        </div><!-- /.repository-sidebar -->

        <div id="js-repo-pjax-container" class="repository-content context-loader-container" data-pjax-container>
          

<a href="/ntnmathur/GettingAndCleaningData/blob/922ac6053ac4574e9117ecb44a22229aca449cff/CodeBook.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:8743b6c0262edc9e32bcee2630bb4c8f -->

<div class="file-navigation">
  
<div class="select-menu js-menu-container js-select-menu left">
  <span class="minibutton select-menu-button js-menu-target css-truncate" data-hotkey="w"
    data-master-branch="master"
    data-ref="master"
    title="master"
    role="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <span class="octicon octicon-git-branch"></span>
    <i>branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </span>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <span class="select-menu-title">Switch branches/tags</span>
        <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
      </div> <!-- /.select-menu-header -->

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" class="js-select-menu-tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" class="js-select-menu-tab">Tags</a>
            </li>
          </ul>
        </div><!-- /.select-menu-tabs -->
      </div><!-- /.select-menu-filters -->

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <div class="select-menu-item js-navigation-item selected">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <a href="/ntnmathur/GettingAndCleaningData/blob/master/CodeBook.md"
                 data-name="master"
                 data-skip-pjax="true"
                 rel="nofollow"
                 class="js-navigation-open select-menu-item-text css-truncate-target"
                 title="master">master</a>
            </div> <!-- /.select-menu-item -->
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div> <!-- /.select-menu-list -->

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div> <!-- /.select-menu-list -->

    </div> <!-- /.select-menu-modal -->
  </div> <!-- /.select-menu-modal-holder -->
</div> <!-- /.select-menu -->

  <div class="button-group right">
    <a href="/ntnmathur/GettingAndCleaningData/find/master"
          class="js-show-file-finder minibutton empty-icon tooltipped tooltipped-s"
          data-pjax
          data-hotkey="t"
          aria-label="Quickly jump between files">
      <span class="octicon octicon-list-unordered"></span>
    </a>
    <button class="js-zeroclipboard minibutton zeroclipboard-button"
          data-clipboard-text="CodeBook.md"
          aria-label="Copy to clipboard"
          data-copied-hint="Copied!">
      <span class="octicon octicon-clippy"></span>
    </button>
  </div>

  <div class="breadcrumb">
    <span class='repo-root js-repo-root'><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/ntnmathur/GettingAndCleaningData" class="" data-branch="master" data-direction="back" data-pjax="true" itemscope="url"><span itemprop="title">GettingAndCleaningData</span></a></span></span><span class="separator"> / </span><strong class="final-path">CodeBook.md</strong>
  </div>
</div>


  <div class="commit file-history-tease">
    <div class="file-history-tease-header">
        <img alt="ntnmathur" class="avatar" data-user="7801923" height="24" src="https://avatars0.githubusercontent.com/u/7801923?v=2&amp;s=48" width="24" />
        <span class="author"><a href="/ntnmathur" rel="author">ntnmathur</a></span>
        <time datetime="2014-09-21T16:08:30-07:00" is="relative-time">September 21, 2014</time>
        <div class="commit-title">
            <a href="/ntnmathur/GettingAndCleaningData/commit/922ac6053ac4574e9117ecb44a22229aca449cff" class="message" data-pjax="true" title="Update CodeBook.md">Update CodeBook.md</a>
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
            <img alt="ntnmathur" data-user="7801923" height="24" src="https://avatars0.githubusercontent.com/u/7801923?v=2&amp;s=48" width="24" />
            <a href="/ntnmathur">ntnmathur</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file-box">
  <div class="file">
    <div class="meta clearfix">
      <div class="info file-name">
          <span>60 lines (43 sloc)</span>
          <span class="meta-divider"></span>
        <span>2.093 kb</span>
      </div>
      <div class="actions">
        <div class="button-group">
          <a href="/ntnmathur/GettingAndCleaningData/raw/master/CodeBook.md" class="minibutton " id="raw-url">Raw</a>
            <a href="/ntnmathur/GettingAndCleaningData/blame/master/CodeBook.md" class="minibutton js-update-url-with-hash">Blame</a>
          <a href="/ntnmathur/GettingAndCleaningData/commits/master/CodeBook.md" class="minibutton " rel="nofollow">History</a>
        </div><!-- /.button-group -->

          <a class="octicon-button tooltipped tooltipped-nw js-conduit-openfile-check"
             href="http://mac.github.com"
             data-url="github-mac://openRepo/https://github.com/ntnmathur/GettingAndCleaningData?branch=master&amp;filepath=CodeBook.md"
             aria-label="Open this file in GitHub for Mac"
             data-failed-title="Your version of GitHub for Mac is too old to open this file. Try checking for updates.">
              <span class="octicon octicon-device-desktop"></span>
          </a>

              <a class="octicon-button tooltipped tooltipped-n js-update-url-with-hash"
                 aria-label="Clicking this button will fork this project so you can edit the file"
                 href="/ntnmathur/GettingAndCleaningData/edit/master/CodeBook.md"
                 data-method="post" rel="nofollow"><span class="octicon octicon-pencil"></span></a>

            <a class="octicon-button danger tooltipped tooltipped-s"
               href="/ntnmathur/GettingAndCleaningData/delete/master/CodeBook.md"
               aria-label="Fork this project and delete file"
               data-method="post" data-test-id="delete-blob-file" rel="nofollow">
          <span class="octicon octicon-trashcan"></span>
        </a>
      </div><!-- /.actions -->
    </div>
      <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1>
<a name="user-content-download-the-zip-file" class="anchor" href="#download-the-zip-file" aria-hidden="true"><span class="octicon octicon-link"></span></a>Download the zip file</h1>

<p>zipfile &lt;- "<a href="https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip">https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip</a>"
download.file(zipfile, destfile = "Dataset.zip", method = "curl")
unzip("Dataset.zip")</p>

<h1>
<a name="user-content-load-activity-labels" class="anchor" href="#load-activity-labels" aria-hidden="true"><span class="octicon octicon-link"></span></a>Load activity labels</h1>

<p>activity_labels &lt;- read.table("./UCI HAR Dataset/activity_labels.txt")[,2]</p>

<h1>
<a name="user-content-load-data-column-names" class="anchor" href="#load-data-column-names" aria-hidden="true"><span class="octicon octicon-link"></span></a>Load data column names</h1>

<p>features &lt;- read.table("./UCI HAR Dataset/features.txt")[,2]</p>

<h1>
<a name="user-content-extract-measurements-on-the-mean-and-standard-deviation-for-each-measurement" class="anchor" href="#extract-measurements-on-the-mean-and-standard-deviation-for-each-measurement" aria-hidden="true"><span class="octicon octicon-link"></span></a>Extract measurements on the mean and standard deviation for each measurement.</h1>

<p>extract_features &lt;- grepl("mean|std", features)</p>

<h1>
<a name="user-content-load-x_test--y_test-data" class="anchor" href="#load-x_test--y_test-data" aria-hidden="true"><span class="octicon octicon-link"></span></a>Load X_test &amp; y_test data.</h1>

<p>X_test &lt;- read.table("./UCI HAR Dataset/test/X_test.txt")
y_test &lt;- read.table("./UCI HAR Dataset/test/y_test.txt")
subject_test &lt;- read.table("./UCI HAR Dataset/test/subject_test.txt")</p>

<p>names(X_test) = features</p>

<h1>
<a name="user-content-extract-the-mean-and-standard-deviation-for-each-measurement" class="anchor" href="#extract-the-mean-and-standard-deviation-for-each-measurement" aria-hidden="true"><span class="octicon octicon-link"></span></a>Extract the mean and standard deviation for each measurement.</h1>

<p>X_test = X_test[,extract_features]</p>

<h1>
<a name="user-content-load-activity-labels-1" class="anchor" href="#load-activity-labels-1" aria-hidden="true"><span class="octicon octicon-link"></span></a>Load activity labels</h1>

<p>y_test[,2] = activity_labels[y_test[,1]]
names(y_test) = c("Activity_ID", "Activity_Label")
names(subject_test) = "subject"</p>

<h1>
<a name="user-content-bind-data" class="anchor" href="#bind-data" aria-hidden="true"><span class="octicon octicon-link"></span></a>Bind data</h1>

<p>test_data &lt;- cbind(as.data.table(subject_test), y_test, X_test)</p>

<h1>
<a name="user-content-load-and-process-x_train--y_train-data" class="anchor" href="#load-and-process-x_train--y_train-data" aria-hidden="true"><span class="octicon octicon-link"></span></a>Load and process X_train &amp; y_train data.</h1>

<p>X_train &lt;- read.table("./UCI HAR Dataset/train/X_train.txt")
y_train &lt;- read.table("./UCI HAR Dataset/train/y_train.txt")</p>

<p>subject_train &lt;- read.table("./UCI HAR Dataset/train/subject_train.txt")
names(X_train) = features</p>

<h1>
<a name="user-content-extract-only-the-measurements-on-the-mean-and-standard-deviation-for-each-measurement" class="anchor" href="#extract-only-the-measurements-on-the-mean-and-standard-deviation-for-each-measurement" aria-hidden="true"><span class="octicon octicon-link"></span></a>Extract only the measurements on the mean and standard deviation for each measurement.</h1>

<p>X_train = X_train[,extract_features]</p>

<h1>
<a name="user-content-load-activity-data" class="anchor" href="#load-activity-data" aria-hidden="true"><span class="octicon octicon-link"></span></a>Load activity data</h1>

<p>y_train[,2] = activity_labels[y_train[,1]]
names(y_train) = c("Activity_ID", "Activity_Label")
names(subject_train) = "subject"</p>

<h1>
<a name="user-content-bind-data-1" class="anchor" href="#bind-data-1" aria-hidden="true"><span class="octicon octicon-link"></span></a>Bind data</h1>

<p>train_data &lt;- cbind(as.data.table(subject_train), y_train, X_train)</p>

<h1>
<a name="user-content-merge-test-and-train-data" class="anchor" href="#merge-test-and-train-data" aria-hidden="true"><span class="octicon octicon-link"></span></a>Merge test and train data</h1>

<p>data = rbind(test_data, train_data)</p>

<p>id_labels   = c("subject", "Activity_ID", "Activity_Label")
data_labels = setdiff(colnames(data), id_labels)
melt_data      = melt(data, id = id_labels, measure.vars = data_labels)</p>

<h1>
<a name="user-content-apply-mean-function-to-dataset-using-dcast-function" class="anchor" href="#apply-mean-function-to-dataset-using-dcast-function" aria-hidden="true"><span class="octicon octicon-link"></span></a>Apply mean function to dataset using dcast function</h1>

<p>tidy_data   = dcast(melt_data, subject + Activity_Label ~ variable, mean)</p></article>
  </div>

  </div>
</div>

<a href="#jump-to-line" rel="facebox[.linejump]" data-hotkey="l" style="display:none">Jump to Line</a>
<div id="jump-to-line" style="display:none">
  <form accept-charset="UTF-8" class="js-jump-to-line-form">
    <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" autofocus>
    <button type="submit" class="button">Go</button>
  </form>
</div>

        </div>

      </div><!-- /.repo-container -->
      <div class="modal-backdrop"></div>
    </div><!-- /.container -->
  </div><!-- /.site -->


    </div><!-- /.wrapper -->

      <div class="container">
  <div class="site-footer">
    <ul class="site-footer-links right">
      <li><a href="https://status.github.com/">Status</a></li>
      <li><a href="http://developer.github.com">API</a></li>
      <li><a href="http://training.github.com">Training</a></li>
      <li><a href="http://shop.github.com">Shop</a></li>
      <li><a href="/blog">Blog</a></li>
      <li><a href="/about">About</a></li>

    </ul>

    <a href="/" aria-label="Homepage">
      <span class="mega-octicon octicon-mark-github" title="GitHub"></span>
    </a>

    <ul class="site-footer-links">
      <li>&copy; 2014 <span title="0.04272s from github-fe118-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="/site/terms">Terms</a></li>
        <li><a href="/site/privacy">Privacy</a></li>
        <li><a href="/security">Security</a></li>
        <li><a href="/contact">Contact</a></li>
    </ul>
  </div><!-- /.site-footer -->
</div><!-- /.container -->


    <div class="fullscreen-overlay js-fullscreen-overlay" id="fullscreen_overlay">
  <div class="fullscreen-container js-suggester-container">
    <div class="textarea-wrap">
      <textarea name="fullscreen-contents" id="fullscreen-contents" class="fullscreen-contents js-fullscreen-contents js-suggester-field" placeholder=""></textarea>
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


      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-aa525778734e809f86b506a9e578025218e40c30.js" type="text/javascript"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-7c08e57fe907469eef667960929fd17ff5f42546.js" type="text/javascript"></script>
      
      
        <script async src="https://www.google-analytics.com/analytics.js"></script>
  </body>
</html>

