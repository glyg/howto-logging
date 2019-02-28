





<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
  <link rel="dns-prefetch" href="https://github.githubassets.com">
  <link rel="dns-prefetch" href="https://avatars0.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars1.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars2.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars3.githubusercontent.com">
  <link rel="dns-prefetch" href="https://github-cloud.s3.amazonaws.com">
  <link rel="dns-prefetch" href="https://user-images.githubusercontent.com/">



  <link crossorigin="anonymous" media="all" integrity="sha512-UFMpXZiU8/kG0aZl62l3OFZi0gwlVRLYrsamBbXttDRSbDmQk1ZyKj5R11ghzrHB/NaIPBuLauI34mVpsuxx5w==" rel="stylesheet" href="https://github.githubassets.com/assets/frameworks-94eca081886beb7440fa7236f4fd103f.css" />
  <link crossorigin="anonymous" media="all" integrity="sha512-FIEp4ofjNZOwIuaCNdkF6w53h1fjud2bVTkAOnOQOL3+uw98WLUVoh+QIC6gJ/fWDkIeNNwkc/+gyn8NUJiWZw==" rel="stylesheet" href="https://github.githubassets.com/assets/site-2a37b0558327c9981d25e3ed83ae9eec.css" />
    <link crossorigin="anonymous" media="all" integrity="sha512-S3WlG8KQvDFCgDsuPGZNJ5t/coqQ7kLvXJW0uD6AXKaB24K8CmQlA3yUslj0cb4aePNv89YTVahRMWLP1N44TQ==" rel="stylesheet" href="https://github.githubassets.com/assets/github-ec46e869112a2c60d943fd503eef6b39.css" />
    
    
    
    

  <meta name="viewport" content="width=device-width">
  
  <title>cpython/logging.rst at master · python/cpython · GitHub</title>
    <meta name="description" content="The Python programming language. Contribute to python/cpython development by creating an account on GitHub.">
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
  <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
  <meta property="fb:app_id" content="1401488693436528">

    
    <meta property="og:image" content="https://avatars2.githubusercontent.com/u/1525981?s=400&amp;v=4" /><meta property="og:site_name" content="GitHub" /><meta property="og:type" content="object" /><meta property="og:title" content="python/cpython" /><meta property="og:url" content="https://github.com/python/cpython" /><meta property="og:description" content="The Python programming language. Contribute to python/cpython development by creating an account on GitHub." />

  <link rel="assets" href="https://github.githubassets.com/">
  
  <meta name="pjax-timeout" content="1000">
  
  <meta name="request-id" content="C912:2E288:12EFBC:1C237C:5C77B5EE" data-pjax-transient>


  

  <meta name="selected-link" value="repo_source" data-pjax-transient>

      <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
    <meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-site-verification" content="GXs5KoUUkNCoaAZn7wPN-t01Pywp9M3sEjnt_3_ZWPc">

  <meta name="octolytics-host" content="collector.githubapp.com" /><meta name="octolytics-app-id" content="github" /><meta name="octolytics-event-url" content="https://collector.githubapp.com/github-external/browser_event" /><meta name="octolytics-dimension-request_id" content="C912:2E288:12EFBC:1C237C:5C77B5EE" /><meta name="octolytics-dimension-region_edge" content="ams" /><meta name="octolytics-dimension-region_render" content="iad" />
<meta name="analytics-location" content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" />



    <meta name="google-analytics" content="UA-3769691-2">


<meta class="js-ga-set" name="dimension1" content="Logged Out">



  

      <meta name="hostname" content="github.com">
    <meta name="user-login" content="">

      <meta name="expected-hostname" content="github.com">
    <meta name="js-proxy-site-detection-payload" content="OWFhMmZlYmJjOTA1MDUwZDJjMWVkZmFlNzZjN2E5NTM4NWNkMzIyMTJlMTgxYTQyZGQ1YmFhYjE5MmFkNjc5ZHx7InJlbW90ZV9hZGRyZXNzIjoiOTIuOTEuMjIxLjIxOCIsInJlcXVlc3RfaWQiOiJDOTEyOjJFMjg4OjEyRUZCQzoxQzIzN0M6NUM3N0I1RUUiLCJ0aW1lc3RhbXAiOjE1NTEzNDkyMzAsImhvc3QiOiJnaXRodWIuY29tIn0=">

    <meta name="enabled-features" content="UNIVERSE_BANNER,MARKETPLACE_SOCIAL_PROOF,MARKETPLACE_PLAN_RESTRICTION_EDITOR,MARKETPLACE_BROWSING_V2">

  <meta name="html-safe-nonce" content="9d371273d9db12993769f01be99be4c0f13c3f38">

  <meta http-equiv="x-pjax-version" content="51633f82d41fbb109c08bc27389aacb1">
  

      <link href="https://github.com/python/cpython/commits/master.atom" rel="alternate" title="Recent Commits to cpython:master" type="application/atom+xml">

  <meta name="go-import" content="github.com/python/cpython git https://github.com/python/cpython.git">

  <meta name="octolytics-dimension-user_id" content="1525981" /><meta name="octolytics-dimension-user_login" content="python" /><meta name="octolytics-dimension-repository_id" content="81598961" /><meta name="octolytics-dimension-repository_nwo" content="python/cpython" /><meta name="octolytics-dimension-repository_public" content="true" /><meta name="octolytics-dimension-repository_is_fork" content="false" /><meta name="octolytics-dimension-repository_network_root_id" content="81598961" /><meta name="octolytics-dimension-repository_network_root_nwo" content="python/cpython" /><meta name="octolytics-dimension-repository_explore_github_marketplace_ci_cta_shown" content="false" />


    <link rel="canonical" href="https://github.com/python/cpython/blob/master/Doc/howto/logging.rst" data-pjax-transient>


  <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">

  <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">

  <link rel="mask-icon" href="https://github.githubassets.com/pinned-octocat.svg" color="#000000">
  <link rel="icon" type="image/x-icon" class="js-site-favicon" href="https://github.githubassets.com/favicon.ico">

<meta name="theme-color" content="#1e2327">




  <link rel="manifest" href="/manifest.json" crossOrigin="use-credentials">

  </head>

  <body class="logged-out env-production page-blob">
    

  <div class="position-relative js-header-wrapper ">
    <a href="#start-of-content" tabindex="1" class="px-2 py-4 bg-blue text-white show-on-focus js-skip-to-content">Skip to content</a>
    <div id="js-pjax-loader-bar" class="pjax-loader-bar"><div class="progress"></div></div>

    
    
    


        
<header class="Header header-logged-out  position-relative f4 py-3" role="banner">
  <div class="container-lg d-flex px-3">
    <div class="d-flex flex-justify-between flex-items-center">
        <a class="mr-4" href="https://github.com/" aria-label="Homepage" data-ga-click="(Logged out) Header, go to homepage, icon:logo-wordmark">
          <svg height="32" class="octicon octicon-mark-github text-white" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
        </a>
    </div>

    <div class="HeaderMenu HeaderMenu--logged-out d-flex flex-justify-between flex-items-center flex-auto">
      <div class="d-none">
        <button class="btn-link js-details-target" type="button" aria-label="Toggle navigation" aria-expanded="false">
          <svg height="24" class="octicon octicon-x text-gray" viewBox="0 0 12 16" version="1.1" width="18" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
        </button>
      </div>

        <nav class="mt-0" aria-label="Global">
          <ul class="d-flex list-style-none">
              <li class=" mr-3 mr-lg-3 edge-item-fix position-relative flex-wrap flex-justify-between d-flex flex-items-center ">
                <details class="HeaderMenu-details details-overlay details-reset width-full">
                  <summary class="HeaderMenu-summary HeaderMenu-link px-0 py-3 border-0 no-wrap  d-inline-block">
                    Why GitHub?
                    <svg x="0px" y="0px" viewBox="0 0 14 8" xml:space="preserve" fill="none" class="icon-chevon-down-mktg position-relative">
                      <path d="M1,1l6.2,6L13,1"></path>
                    </svg>
                  </summary>
                  <div class="dropdown-menu flex-auto rounded-1 bg-white px-0 mt-0  p-4 left-n4 position-absolute">
                    <a href="/features" class="py-2 lh-condensed-ultra d-block link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Features">Features <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a>
                    <ul class="list-style-none f5 pb-3">
                      <li class="edge-item-fix"><a href="/features/code-review/" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Code review">Code review</a></li>
                      <li class="edge-item-fix"><a href="/features/project-management/" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Project management">Project management</a></li>
                      <li class="edge-item-fix"><a href="/features/integrations" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Integrations">Integrations</a></li>
                      <li class="edge-item-fix"><a href="/features/actions" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Actions">Actions</a>
                      <li class="edge-item-fix"><a href="/features#team-management" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Team management">Team management</a></li>
                      <li class="edge-item-fix"><a href="/features#social-coding" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Social coding">Social coding</a></li>
                      <li class="edge-item-fix"><a href="/features#documentation" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Documentation">Documentation</a></li>
                      <li class="edge-item-fix"><a href="/features#code-hosting" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Code hosting">Code hosting</a></li>
                    </ul>

                    <ul class="list-style-none mb-0 border-lg-top pt-lg-3">
                      <li class="edge-item-fix"><a href="/case-studies" class="py-2 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Case studies">Case Studies <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                      <li class="edge-item-fix"><a href="/security" class="py-2 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Security">Security <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                    </ul>
                  </div>
                </details>
              </li>
              <li class=" mr-3 mr-lg-3">
                <a href="/enterprise" class="HeaderMenu-link no-underline py-3 d-block d-lg-inline-block" data-ga-click="(Logged out) Header, click, go to Enterprise">Enterprise</a>
              </li>

              <li class=" mr-3 mr-lg-3 edge-item-fix position-relative flex-wrap flex-justify-between d-flex flex-items-center ">
                <details class="HeaderMenu-details details-overlay details-reset width-full">
                  <summary class="HeaderMenu-summary HeaderMenu-link px-0 py-3 border-0 no-wrap  d-inline-block">
                    Explore
                    <svg x="0px" y="0px" viewBox="0 0 14 8" xml:space="preserve" fill="none" class="icon-chevon-down-mktg position-relative">
                      <path d="M1,1l6.2,6L13,1"></path>
                    </svg>
                  </summary>

                  <div class="dropdown-menu flex-auto rounded-1 bg-white px-0 pt-2 pb-0 mt-0  p-4 left-n4 position-absolute">
                    <ul class="list-style-none mb-3">
                      <li class="edge-item-fix"><a href="/explore" class="py-2 lh-condensed-ultra d-block link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Features">Explore GitHub <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                    </ul>

                    <h4 class="text-gray-light text-normal text-mono f5 mb-2  border-top pt-3">Learn &amp; contribute</h4>
                    <ul class="list-style-none mb-3">
                      <li class="edge-item-fix"><a href="/topics" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Topics">Topics</a></li>
                      <li class="edge-item-fix"><a href="/collections" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Collections">Collections</a></li>
                      <li class="edge-item-fix"><a href="/trending" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Trending">Trending</a></li>
                      <li class="edge-item-fix"><a href="https://lab.github.com/" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Learning lab">Learning Lab</a></li>
                      <li class="edge-item-fix"><a href="https://opensource.guide" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Open source guides">Open source guides</a></li>
                    </ul>

                    <h4 class="text-gray-light text-normal text-mono f5 mb-2  border-top pt-3">Connect with others</h4>
                    <ul class="list-style-none mb-0">
                      <li class="edge-item-fix"><a href="/events" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Events">Events</a></li>
                      <li class="edge-item-fix"><a href="https://github.community" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Community forum">Community forum</a></li>
                      <li class="edge-item-fix"><a href="https://education.github.com" class="py-2 pb-0 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to GitHub Education">GitHub Education</a></li>
                    </ul>
                  </div>
                </details>
              </li>

              <li class=" mr-3 mr-lg-3">
                <a href="/marketplace" class="HeaderMenu-link no-underline py-3 d-block d-lg-inline-block" data-ga-click="(Logged out) Header, go to Marketplace">Marketplace</a>
              </li>

              <li class=" mr-3 mr-lg-3 edge-item-fix position-relative flex-wrap flex-justify-between d-flex flex-items-center ">
                <details class="HeaderMenu-details details-overlay details-reset width-full">
                  <summary class="HeaderMenu-summary HeaderMenu-link px-0 py-3 border-0 no-wrap  d-inline-block">
                    Pricing
                    <svg x="0px" y="0px" viewBox="0 0 14 8" xml:space="preserve" fill="none" class="icon-chevon-down-mktg position-relative">
                       <path d="M1,1l6.2,6L13,1"></path>
                    </svg>
                  </summary>

                  <div class="dropdown-menu flex-auto rounded-1 bg-white px-0 pt-2 pb-4 mt-0  p-4 left-n4 position-absolute">
                    <a href="/pricing" class="pb-2 lh-condensed-ultra d-block link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Pricing">Plans <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a>

                    <ul class="list-style-none mb-3">
                      <li class="edge-item-fix"><a href="/pricing#feature-comparison" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Compare features">Compare plans</a></li>
                      <li class="edge-item-fix"><a href="https://enterprise.github.com/contact" class="py-2 lh-condensed-ultra d-block link-gray no-underline f5" data-ga-click="(Logged out) Header, go to Compare features">Contact Sales</a></li>
                    </ul>

                    <ul class="list-style-none mb-0  border-top pt-3">
                      <li class="edge-item-fix"><a href="/nonprofit" class="py-2 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover" data-ga-click="(Logged out) Header, go to Nonprofits">Nonprofit <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                      <li class="edge-item-fix"><a href="https://education.github.com" class="py-2 pb-0 lh-condensed-ultra d-block no-underline link-gray-dark no-underline h5 Bump-link--hover"  data-ga-click="(Logged out) Header, go to Education">Education <span class="Bump-link-symbol float-right text-normal text-gray-light">&rarr;</span></a></li>
                    </ul>
                  </div>
                </details>
              </li>
          </ul>
        </nav>

      <div class="d-flex flex-items-center px-0 text-center text-left">
          <div class="d-lg-flex mr-3">
            <div class="header-search scoped-search site-scoped-search js-site-search position-relative js-jump-to"
  role="combobox"
  aria-owns="jump-to-results"
  aria-label="Search or jump to"
  aria-haspopup="listbox"
  aria-expanded="false"
>
  <div class="position-relative">
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-site-search-form" role="search" aria-label="Site" data-scope-type="Repository" data-scope-id="81598961" data-scoped-search-url="/python/cpython/search" data-unscoped-search-url="/search" action="/python/cpython/search" accept-charset="UTF-8" method="get"><input name="utf8" type="hidden" value="&#x2713;" />
      <label class="form-control header-search-wrapper header-search-wrapper-jump-to position-relative d-flex flex-justify-between flex-items-center js-chromeless-input-container">
        <input type="text"
          class="form-control header-search-input jump-to-field js-jump-to-field js-site-search-focus js-site-search-field is-clearable"
          data-hotkey="s,/"
          name="q"
          value=""
          placeholder="Search"
          data-unscoped-placeholder="Search GitHub"
          data-scoped-placeholder="Search"
          autocapitalize="off"
          aria-autocomplete="list"
          aria-controls="jump-to-results"
          aria-label="Search"
          data-jump-to-suggestions-path="/_graphql/GetSuggestedNavigationDestinations#csrf-token=i3tThhx1GjZdx7Gacx4ebfXV2b+BPZ8GWqt122+tU3muRnAa4vHSgHIAG5pyx6g/qWmDuLxDPdJkPjvmragmfw=="
          spellcheck="false"
          autocomplete="off"
          >
          <input type="hidden" class="js-site-search-type-field" name="type" >
            <img src="https://github.githubassets.com/images/search-key-slash.svg" alt="" class="mr-2 header-search-key-slash">

            <div class="Box position-absolute overflow-hidden d-none jump-to-suggestions js-jump-to-suggestions-container">
              
<ul class="d-none js-jump-to-suggestions-template-container">
  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-suggestion" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg height="16" width="16" class="octicon octicon-repo flex-shrink-0 js-jump-to-octicon-repo d-none" title="Repository" aria-label="Repository" viewBox="0 0 12 16" version="1.1" role="img"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-project flex-shrink-0 js-jump-to-octicon-project d-none" title="Project" aria-label="Project" viewBox="0 0 15 16" version="1.1" role="img"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-search flex-shrink-0 js-jump-to-octicon-search d-none" title="Search" aria-label="Search" viewBox="0 0 16 16" version="1.1" role="img"><path fill-rule="evenodd" d="M15.7 13.3l-3.81-3.83A5.93 5.93 0 0 0 13 6c0-3.31-2.69-6-6-6S1 2.69 1 6s2.69 6 6 6c1.3 0 2.48-.41 3.47-1.11l3.83 3.81c.19.2.45.3.7.3.25 0 .52-.09.7-.3a.996.996 0 0 0 0-1.41v.01zM7 10.7c-2.59 0-4.7-2.11-4.7-4.7 0-2.59 2.11-4.7 4.7-4.7 2.59 0 4.7 2.11 4.7 4.7 0 2.59-2.11 4.7-4.7 4.7z"/></svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>

</ul>

<ul class="d-none js-jump-to-no-results-template-container">
  <li class="d-flex flex-justify-center flex-items-center f5 d-none js-jump-to-suggestion p-2">
    <span class="text-gray">No suggested jump to results</span>
  </li>
</ul>

<ul id="jump-to-results" role="listbox" class="p-0 m-0 js-navigation-container jump-to-suggestions-results-container js-jump-to-suggestions-results-container">
  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-scoped-search d-none" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg height="16" width="16" class="octicon octicon-repo flex-shrink-0 js-jump-to-octicon-repo d-none" title="Repository" aria-label="Repository" viewBox="0 0 12 16" version="1.1" role="img"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-project flex-shrink-0 js-jump-to-octicon-project d-none" title="Project" aria-label="Project" viewBox="0 0 15 16" version="1.1" role="img"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-search flex-shrink-0 js-jump-to-octicon-search d-none" title="Search" aria-label="Search" viewBox="0 0 16 16" version="1.1" role="img"><path fill-rule="evenodd" d="M15.7 13.3l-3.81-3.83A5.93 5.93 0 0 0 13 6c0-3.31-2.69-6-6-6S1 2.69 1 6s2.69 6 6 6c1.3 0 2.48-.41 3.47-1.11l3.83 3.81c.19.2.45.3.7.3.25 0 .52-.09.7-.3a.996.996 0 0 0 0-1.41v.01zM7 10.7c-2.59 0-4.7-2.11-4.7-4.7 0-2.59 2.11-4.7 4.7-4.7 2.59 0 4.7 2.11 4.7 4.7 0 2.59-2.11 4.7-4.7 4.7z"/></svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>

  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-global-search d-none" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg height="16" width="16" class="octicon octicon-repo flex-shrink-0 js-jump-to-octicon-repo d-none" title="Repository" aria-label="Repository" viewBox="0 0 12 16" version="1.1" role="img"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-project flex-shrink-0 js-jump-to-octicon-project d-none" title="Project" aria-label="Project" viewBox="0 0 15 16" version="1.1" role="img"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
      <svg height="16" width="16" class="octicon octicon-search flex-shrink-0 js-jump-to-octicon-search d-none" title="Search" aria-label="Search" viewBox="0 0 16 16" version="1.1" role="img"><path fill-rule="evenodd" d="M15.7 13.3l-3.81-3.83A5.93 5.93 0 0 0 13 6c0-3.31-2.69-6-6-6S1 2.69 1 6s2.69 6 6 6c1.3 0 2.48-.41 3.47-1.11l3.83 3.81c.19.2.45.3.7.3.25 0 .52-.09.7-.3a.996.996 0 0 0 0-1.41v.01zM7 10.7c-2.59 0-4.7-2.11-4.7-4.7 0-2.59 2.11-4.7 4.7-4.7 2.59 0 4.7 2.11 4.7 4.7 0 2.59-2.11 4.7-4.7 4.7z"/></svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>


</ul>

            </div>
      </label>
</form>  </div>
</div>

          </div>

        <a class="HeaderMenu-link no-underline mr-3" href="/login?return_to=%2Fpython%2Fcpython%2Fblob%2Fmaster%2FDoc%2Fhowto%2Flogging.rst" data-ga-click="(Logged out) Header, clicked Sign in, text:sign-in">Sign&nbsp;in</a>
          <a class="HeaderMenu-link d-inline-block no-underline border border-gray-dark rounded-1 px-2 py-1" href="/join" data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">Sign&nbsp;up</a>
      </div>
    </div>
  </div>
</header>

  </div>

  <div id="start-of-content" class="show-on-focus"></div>

    <div id="js-flash-container">

</div>



  <div class="application-main " data-commit-hovercards-enabled>
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode" class="">
    <main id="js-repo-pjax-container" data-pjax-container >
      


  


  




  <div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav  ">
    <div class="repohead-details-container clearfix container">

      <ul class="pagehead-actions">


  <li>
      <a href="/login?return_to=%2Fpython%2Fcpython"
    class="btn btn-sm btn-with-count tooltipped tooltipped-s"
    aria-label="You must be signed in to watch a repository" rel="nofollow">
    <svg class="octicon octicon-eye v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
    Watch
  </a>
  <a class="social-count" href="/python/cpython/watchers"
     aria-label="1042 users are watching this repository">
    1,042
  </a>

  </li>

  <li>
        <a href="/login?return_to=%2Fpython%2Fcpython"
      class="btn btn-sm btn-with-count tooltipped tooltipped-s"
      aria-label="You must be signed in to star a repository" rel="nofollow">
      <svg class="octicon octicon-star v-align-text-bottom" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74L14 6z"/></svg>
      Star
    </a>

    <a class="social-count js-social-count" href="/python/cpython/stargazers"
      aria-label="22698 users starred this repository">
      22,698
    </a>

  </li>

  <li>
      <a href="/login?return_to=%2Fpython%2Fcpython"
        class="btn btn-sm btn-with-count tooltipped tooltipped-s"
        aria-label="You must be signed in to fork a repository" rel="nofollow">
        <svg class="octicon octicon-repo-forked v-align-text-bottom" viewBox="0 0 10 16" version="1.1" width="10" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 1a1.993 1.993 0 0 0-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 0 0 2 1a1.993 1.993 0 0 0-1 3.72V6.5l3 3v1.78A1.993 1.993 0 0 0 5 15a1.993 1.993 0 0 0 1-3.72V9.5l3-3V4.72A1.993 1.993 0 0 0 8 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
        Fork
      </a>

    <a href="/python/cpython/network/members" class="social-count"
       aria-label="8784 users forked this repository">
      8,784
    </a>
  </li>
</ul>

      <h1 class="public ">
  <svg class="octicon octicon-repo" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
  <span class="author" itemprop="author"><a class="url fn" rel="author" data-hovercard-type="organization" data-hovercard-url="/orgs/python/hovercard" href="/python">python</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a data-pjax="#js-repo-pjax-container" href="/python/cpython">cpython</a></strong>

</h1>

    </div>
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax container"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
    aria-label="Repository"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a class="js-selected-navigation-item selected reponav-item" itemprop="url" data-hotkey="g c" aria-current="page" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches repo_packages /python/cpython" href="/python/cpython">
      <svg class="octicon octicon-code" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"/></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>


  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a data-hotkey="g p" itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_pulls checks /python/cpython/pulls" href="/python/cpython/pulls">
      <svg class="octicon octicon-git-pull-request" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0 0 10 15a1.993 1.993 0 0 0 1-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v6.56A1.993 1.993 0 0 0 2 15a1.993 1.993 0 0 0 1-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
      <span itemprop="name">Pull requests</span>
      <span class="Counter">1,037</span>
      <meta itemprop="position" content="3">
</a>  </span>





    <a class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors dependency_graph pulse alerts security people /python/cpython/pulse" href="/python/cpython/pulse">
      <svg class="octicon octicon-graph" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"/></svg>
      Insights
</a>

</nav>


  </div>
<div class="container new-discussion-timeline experiment-repo-nav  ">
  <div class="repository-content ">

    
    



  
    <a class="d-none js-permalink-shortcut" data-hotkey="y" href="/python/cpython/blob/4173772031747a9b249be4100b4aa9eda805ea23/Doc/howto/logging.rst">Permalink</a>

    <!-- blob contrib key: blob_contributors:v21:6969ef190ef36303eb11066021bb3a96 -->

        <div class="signup-prompt-bg rounded-1">
      <div class="signup-prompt p-4 text-center mb-4 rounded-1">
        <div class="position-relative">
          <!-- '"` --><!-- </textarea></xmp> --></option></form><form action="/site/dismiss_signup_prompt" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="qjsR+m0iGkzWf7sX71ZpzSXqDTMIdn86oUKxUX6I5Sy7gyHLfTNoblEI7g6vdE3p9Vp2qIg9T1RT8znU4//vow==" />
            <button type="submit" class="position-absolute top-0 right-0 btn-link link-gray" data-ga-click="(Logged out) Sign up prompt, clicked Dismiss, text:dismiss">
              Dismiss
            </button>
</form>          <h3 class="pt-2">Join GitHub today</h3>
          <p class="col-6 mx-auto">GitHub is home to over 31 million developers working together to host and review code, manage projects, and build software together.</p>
          <a class="btn btn-primary" href="/join?source=prompt-blob-show" data-ga-click="(Logged out) Sign up prompt, clicked Sign up, text:sign-up">Sign up</a>
        </div>
      </div>
    </div>


    <div class="file-navigation">
      
<details class="details-reset details-overlay select-menu branch-select-menu float-left">
  <summary class="btn btn-sm select-menu-button css-truncate"
           data-hotkey="w"
           
           title="Switch branches or tags">
    <i>Branch:</i>
    <span class="css-truncate-target">master</span>
  </summary>

  <details-menu class="select-menu-modal position-absolute" style="z-index: 99;" src="/python/cpython/ref-list/master/Doc/howto/logging.rst?source_action=show&amp;source_controller=blob" preload>
    <include-fragment class="select-menu-loading-overlay anim-pulse">
      <svg height="32" class="octicon octicon-octoface" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M14.7 5.34c.13-.32.55-1.59-.13-3.31 0 0-1.05-.33-3.44 1.3-1-.28-2.07-.32-3.13-.32s-2.13.04-3.13.32c-2.39-1.64-3.44-1.3-3.44-1.3-.68 1.72-.26 2.99-.13 3.31C.49 6.21 0 7.33 0 8.69 0 13.84 3.33 15 7.98 15S16 13.84 16 8.69c0-1.36-.49-2.48-1.3-3.35zM8 14.02c-3.3 0-5.98-.15-5.98-3.35 0-.76.38-1.48 1.02-2.07 1.07-.98 2.9-.46 4.96-.46 2.07 0 3.88-.52 4.96.46.65.59 1.02 1.3 1.02 2.07 0 3.19-2.68 3.35-5.98 3.35zM5.49 9.01c-.66 0-1.2.8-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.54-1.78-1.2-1.78zm5.02 0c-.66 0-1.2.79-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.53-1.78-1.2-1.78z"/></svg>
    </include-fragment>
  </details-menu>
</details>

      <div class="BtnGroup float-right">
        <a href="/python/cpython/find/master"
              class="js-pjax-capture-input btn btn-sm BtnGroup-item"
              data-pjax
              data-hotkey="t">
          Find file
        </a>
        <clipboard-copy for="blob-path" class="btn btn-sm BtnGroup-item">
          Copy path
        </clipboard-copy>
      </div>
      <div id="blob-path" class="breadcrumb">
        <span class="repo-root js-repo-root"><span class="js-path-segment"><a data-pjax="true" href="/python/cpython"><span>cpython</span></a></span></span><span class="separator">/</span><span class="js-path-segment"><a data-pjax="true" href="/python/cpython/tree/master/Doc"><span>Doc</span></a></span><span class="separator">/</span><span class="js-path-segment"><a data-pjax="true" href="/python/cpython/tree/master/Doc/howto"><span>howto</span></a></span><span class="separator">/</span><strong class="final-path">logging.rst</strong>
      </div>
    </div>


    
  <div class="commit-tease d-flex flex-column">
      <div class="d-flex flex-justify-between ">
        <span class="pr-md-4">
          <a rel="contributor" data-skip-pjax="true" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=6350027" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/yuji38kwmt"><img class="avatar" src="https://avatars0.githubusercontent.com/u/6350027?s=40&amp;v=4" width="20" height="20" alt="@yuji38kwmt" /></a>
          <a class="user-mention" rel="contributor" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=6350027" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/yuji38kwmt">yuji38kwmt</a>
            <a data-pjax="true" title="bpo-35781: Changed references to deprecated &#39;warn&#39; method in logging documentation in favour of &#39;warning&#39; (GH-11654)" class="message" href="/python/cpython/commit/cda73a5af2ff064ca82140342b3158851d43868f">bpo-35781: Changed references to deprecated 'warn' method in logging …</a>
        </span>
        <span class="d-inline-block flex-shrink-0 v-align-bottom ">
          <a class="commit-tease-sha pr-2" href="/python/cpython/commit/cda73a5af2ff064ca82140342b3158851d43868f" data-pjax>
            cda73a5
          </a>
          <relative-time datetime="2019-01-23T07:27:13Z">Jan 23, 2019</relative-time>
        </span>
      </div>

    <div class="commit-tease-contributors flex-auto">
      
<details class="details-reset details-overlay details-overlay-dark lh-default text-gray-dark float-left mr-2" id="blob_contributors_box">
  <summary
      class="btn-link"
      aria-haspopup="dialog"
      
      
      >
    
    <span><strong>9</strong> contributors</span>
  </summary>
  <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast " aria-label="Users who have contributed to this file">
    <div class="Box-header">
      <button class="Box-btn-octicon btn-octicon float-right" type="button" aria-label="Close dialog" data-close-dialog>
        <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
      </button>
      <h3 class="Box-title">Users who have contributed to this file</h3>
    </div>
    
        <ul class="list-style-none overflow-auto">
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/vsajip">
                <img class="avatar mr-2" alt="" src="https://avatars1.githubusercontent.com/u/130553?s=40&amp;v=4" width="20" height="20" />
                vsajip
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/serhiy-storchaka">
                <img class="avatar mr-2" alt="" src="https://avatars0.githubusercontent.com/u/3659035?s=40&amp;v=4" width="20" height="20" />
                serhiy-storchaka
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/birkenfeld">
                <img class="avatar mr-2" alt="" src="https://avatars2.githubusercontent.com/u/144359?s=40&amp;v=4" width="20" height="20" />
                birkenfeld
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/Natim">
                <img class="avatar mr-2" alt="" src="https://avatars1.githubusercontent.com/u/229453?s=40&amp;v=4" width="20" height="20" />
                Natim
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/CuriousLearner">
                <img class="avatar mr-2" alt="" src="https://avatars0.githubusercontent.com/u/8039608?s=40&amp;v=4" width="20" height="20" />
                CuriousLearner
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/yuji38kwmt">
                <img class="avatar mr-2" alt="" src="https://avatars0.githubusercontent.com/u/6350027?s=40&amp;v=4" width="20" height="20" />
                yuji38kwmt
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/vadmium">
                <img class="avatar mr-2" alt="" src="https://avatars2.githubusercontent.com/u/1024659?s=40&amp;v=4" width="20" height="20" />
                vadmium
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/merwok">
                <img class="avatar mr-2" alt="" src="https://avatars3.githubusercontent.com/u/635179?s=40&amp;v=4" width="20" height="20" />
                merwok
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/maggyero">
                <img class="avatar mr-2" alt="" src="https://avatars1.githubusercontent.com/u/33548838?s=40&amp;v=4" width="20" height="20" />
                maggyero
</a>            </li>
        </ul>

  </details-dialog>
</details>
          <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=130553" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging.rst?author=vsajip">
      <img class="avatar" src="https://avatars1.githubusercontent.com/u/130553?s=40&amp;v=4" width="20" height="20" alt="@vsajip" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=3659035" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging.rst?author=serhiy-storchaka">
      <img class="avatar" src="https://avatars0.githubusercontent.com/u/3659035?s=40&amp;v=4" width="20" height="20" alt="@serhiy-storchaka" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=144359" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging.rst?author=birkenfeld">
      <img class="avatar" src="https://avatars2.githubusercontent.com/u/144359?s=40&amp;v=4" width="20" height="20" alt="@birkenfeld" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=229453" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging.rst?author=Natim">
      <img class="avatar" src="https://avatars1.githubusercontent.com/u/229453?s=40&amp;v=4" width="20" height="20" alt="@Natim" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=8039608" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging.rst?author=CuriousLearner">
      <img class="avatar" src="https://avatars0.githubusercontent.com/u/8039608?s=40&amp;v=4" width="20" height="20" alt="@CuriousLearner" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=6350027" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging.rst?author=yuji38kwmt">
      <img class="avatar" src="https://avatars0.githubusercontent.com/u/6350027?s=40&amp;v=4" width="20" height="20" alt="@yuji38kwmt" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=1024659" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging.rst?author=vadmium">
      <img class="avatar" src="https://avatars2.githubusercontent.com/u/1024659?s=40&amp;v=4" width="20" height="20" alt="@vadmium" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=635179" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging.rst?author=merwok">
      <img class="avatar" src="https://avatars3.githubusercontent.com/u/635179?s=40&amp;v=4" width="20" height="20" alt="@merwok" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=33548838" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging.rst?author=maggyero">
      <img class="avatar" src="https://avatars1.githubusercontent.com/u/33548838?s=40&amp;v=4" width="20" height="20" alt="@maggyero" /> 
</a>

    </div>
  </div>





    <div class="file ">
      
<div class="file-header ">
  
  <div class="file-info float-left ">
      1104 lines (836 sloc)
      <span class="file-info-divider"></span>
    46.7 KB
  </div>

  <div class="file-actions d-flex ">

    <div class="BtnGroup">
      <a id="raw-url" class="btn btn-sm BtnGroup-item" href="/python/cpython/raw/master/Doc/howto/logging.rst">Raw</a>
        <a class="btn btn-sm js-update-url-with-hash BtnGroup-item" data-hotkey="b" href="/python/cpython/blame/master/Doc/howto/logging.rst">Blame</a>
      <a rel="nofollow" class="btn btn-sm BtnGroup-item" href="/python/cpython/commits/master/Doc/howto/logging.rst">History</a>
    </div>


    <div>

          <button type="button" class="btn-octicon disabled tooltipped tooltipped-nw"
            aria-label="You must be signed in to make or propose changes">
            <svg class="octicon octicon-pencil" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 0 1 1.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"/></svg>
          </button>
          <button type="button" class="btn-octicon btn-octicon-danger disabled tooltipped tooltipped-nw"
            aria-label="You must be signed in to make or propose changes">
            <svg class="octicon octicon-trashcan" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"/></svg>
          </button>
    </div>
  </div>
</div>

      
  <div id="readme" class="readme blob instapaper_body js-code-block-container">
    <article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-logging-howto" class="anchor" aria-hidden="true" href="#logging-howto"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Logging HOWTO</h1>
<table frame="void" rules="none">


<tbody valign="top">
<tr><th>Author:</th>
<td>Vinay Sajip &lt;vinay_sajip at red-dove dot com&gt;</td></tr>
</tbody>
</table>
<pre>.. currentmodule:: logging

</pre>
<a name="user-content-basic-logging-tutorial"></a>
<h2><a id="user-content-basic-logging-tutorial" class="anchor" aria-hidden="true" href="#basic-logging-tutorial"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Basic Logging Tutorial</h2>
<p>Logging is a means of tracking events that happen when some software runs. The
software's developer adds logging calls to their code to indicate that certain
events have occurred. An event is described by a descriptive message which can
optionally contain variable data (i.e. data that is potentially different for
each occurrence of the event). Events also have an importance which the
developer ascribes to the event; the importance can also be called the <em>level</em>
or <em>severity</em>.</p>
<a name="user-content-when-to-use-logging"></a>
<h3><a id="user-content-when-to-use-logging" class="anchor" aria-hidden="true" href="#when-to-use-logging"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>When to use logging</h3>
<p>Logging provides a set of convenience functions for simple logging usage. These
are <a href="#id1"><span id="user-content-id2">:func:`debug`</span></a>, <a href="#id3"><span id="user-content-id4">:func:`info`</span></a>, <a href="#id5"><span id="user-content-id6">:func:`warning`</span></a>, <a href="#id7"><span id="user-content-id8">:func:`error`</span></a> and
<a href="#id9"><span id="user-content-id10">:func:`critical`</span></a>. To determine when to use logging, see the table below, which
states, for each of a set of common tasks, the best tool to use for it.</p>
<table>




<thead valign="bottom">
<tr><th>Task you want to perform</th>
<th>The best tool for the task</th>
</tr>
</thead>
<tbody valign="top">
<tr><td>Display console output for ordinary
usage of a command line script or
program</td>
<td><a href="#id11"><span id="user-content-id12">:func:`print`</span></a></td>
</tr>
<tr><td>Report events that occur during
normal operation of a program (e.g.
for status monitoring or fault
investigation)</td>
<td><a href="#id13"><span id="user-content-id14">:func:`logging.info`</span></a> (or
<a href="#id15"><span id="user-content-id16">:func:`logging.debug`</span></a> for very
detailed output for diagnostic
purposes)</td>
</tr>
<tr><td>Issue a warning regarding a
particular runtime event</td>
<td><p><a href="#id17"><span id="user-content-id18">:func:`warnings.warn`</span></a> in library
code if the issue is avoidable and
the client application should be
modified to eliminate the warning</p>
<p><a href="#id19"><span id="user-content-id20">:func:`logging.warning`</span></a> if there is
nothing the client application can do
about the situation, but the event
should still be noted</p>
</td>
</tr>
<tr><td>Report an error regarding a
particular runtime event</td>
<td>Raise an exception</td>
</tr>
<tr><td>Report suppression of an error
without raising an exception (e.g.
error handler in a long-running
server process)</td>
<td><a href="#id21"><span id="user-content-id22">:func:`logging.error`</span></a>,
<a href="#id23"><span id="user-content-id24">:func:`logging.exception`</span></a> or
<a href="#id25"><span id="user-content-id26">:func:`logging.critical`</span></a> as
appropriate for the specific error
and application domain</td>
</tr>
</tbody>
</table>
<p>The logging functions are named after the level or severity of the events
they are used to track. The standard levels and their applicability are
described below (in increasing order of severity):</p>
<pre>.. tabularcolumns:: |l|L|

</pre>
<table>




<thead valign="bottom">
<tr><th>Level</th>
<th>When it's used</th>
</tr>
</thead>
<tbody valign="top">
<tr><td><code>DEBUG</code></td>
<td>Detailed information, typically of interest
only when diagnosing problems.</td>
</tr>
<tr><td><code>INFO</code></td>
<td>Confirmation that things are working as
expected.</td>
</tr>
<tr><td><code>WARNING</code></td>
<td>An indication that something unexpected
happened, or indicative of some problem in
the near future (e.g. 'disk space low').
The software is still working as expected.</td>
</tr>
<tr><td><code>ERROR</code></td>
<td>Due to a more serious problem, the software
has not been able to perform some function.</td>
</tr>
<tr><td><code>CRITICAL</code></td>
<td>A serious error, indicating that the program
itself may be unable to continue running.</td>
</tr>
</tbody>
</table>
<p>The default level is <code>WARNING</code>, which means that only events of this level
and above will be tracked, unless the logging package is configured to do
otherwise.</p>
<p>Events that are tracked can be handled in different ways. The simplest way of
handling tracked events is to print them to the console. Another common way
is to write them to a disk file.</p>
<a name="user-content-a-simple-example"></a>
<h3><a id="user-content-a-simple-example" class="anchor" aria-hidden="true" href="#a-simple-example"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>A simple example</h3>
<p>A very simple example is:</p>
<pre>import logging
logging.warning('Watch out!')  # will print a message to the console
logging.info('I told you so')  # will not print anything
</pre>
<p>If you type these lines into a script and run it, you'll see:</p>
<pre lang="none">WARNING:root:Watch out!
</pre>
<p>printed out on the console. The <code>INFO</code> message doesn't appear because the
default level is <code>WARNING</code>. The printed message includes the indication of
the level and the description of the event provided in the logging call, i.e.
'Watch out!'. Don't worry about the 'root' part for now: it will be explained
later. The actual output can be formatted quite flexibly if you need that;
formatting options will also be explained later.</p>
<a name="user-content-logging-to-a-file"></a>
<h3><a id="user-content-logging-to-a-file" class="anchor" aria-hidden="true" href="#logging-to-a-file"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Logging to a file</h3>
<p>A very common situation is that of recording logging events in a file, so let's
look at that next. Be sure to try the following in a newly-started Python
interpreter, and don't just continue from the session described above:</p>
<pre>import logging
logging.basicConfig(filename='example.log',level=logging.DEBUG)
logging.debug('This message should go to the log file')
logging.info('So should this')
logging.warning('And this, too')
</pre>
<p>And now if we open the file and look at what we have, we should find the log
messages:</p>
<pre lang="none">DEBUG:root:This message should go to the log file
INFO:root:So should this
WARNING:root:And this, too
</pre>
<p>This example also shows how you can set the logging level which acts as the
threshold for tracking. In this case, because we set the threshold to
<code>DEBUG</code>, all of the messages were printed.</p>
<p>If you want to set the logging level from a command-line option such as:</p>
<pre lang="none">--log=INFO
</pre>
<p>and you have the value of the parameter passed for <code>--log</code> in some variable
<em>loglevel</em>, you can use:</p>
<pre>getattr(logging, loglevel.upper())
</pre>
<p>to get the value which you'll pass to <a href="#id27"><span id="user-content-id28">:func:`basicConfig`</span></a> via the <em>level</em>
argument. You may want to error check any user input value, perhaps as in the
following example:</p>
<pre># assuming loglevel is bound to the string value obtained from the
# command line argument. Convert to upper case to allow the user to
# specify --log=DEBUG or --log=debug
numeric_level = getattr(logging, loglevel.upper(), None)
if not isinstance(numeric_level, int):
    raise ValueError('Invalid log level: %s' % loglevel)
logging.basicConfig(level=numeric_level, ...)
</pre>
<p>The call to <a href="#id29"><span id="user-content-id30">:func:`basicConfig`</span></a> should come <em>before</em> any calls to <a href="#id31"><span id="user-content-id32">:func:`debug`</span></a>,
<a href="#id33"><span id="user-content-id34">:func:`info`</span></a> etc. As it's intended as a one-off simple configuration facility,
only the first call will actually do anything: subsequent calls are effectively
no-ops.</p>
<p>If you run the above script several times, the messages from successive runs
are appended to the file <em>example.log</em>. If you want each run to start afresh,
not remembering the messages from earlier runs, you can specify the <em>filemode</em>
argument, by changing the call in the above example to:</p>
<pre>logging.basicConfig(filename='example.log', filemode='w', level=logging.DEBUG)
</pre>
<p>The output will be the same as before, but the log file is no longer appended
to, so the messages from earlier runs are lost.</p>
<a name="user-content-logging-from-multiple-modules"></a>
<h3><a id="user-content-logging-from-multiple-modules" class="anchor" aria-hidden="true" href="#logging-from-multiple-modules"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Logging from multiple modules</h3>
<p>If your program consists of multiple modules, here's an example of how you
could organize logging in it:</p>
<pre># myapp.py
import logging
import mylib

def main():
    logging.basicConfig(filename='myapp.log', level=logging.INFO)
    logging.info('Started')
    mylib.do_something()
    logging.info('Finished')

if __name__ == '__main__':
    main()
</pre>
<pre># mylib.py
import logging

def do_something():
    logging.info('Doing something')
</pre>
<p>If you run <em>myapp.py</em>, you should see this in <em>myapp.log</em>:</p>
<pre lang="none">INFO:root:Started
INFO:root:Doing something
INFO:root:Finished
</pre>
<p>which is hopefully what you were expecting to see. You can generalize this to
multiple modules, using the pattern in <em>mylib.py</em>. Note that for this simple
usage pattern, you won't know, by looking in the log file, <em>where</em> in your
application your messages came from, apart from looking at the event
description. If you want to track the location of your messages, you'll need
to refer to the documentation beyond the tutorial level -- see
<a href="#id35"><span id="user-content-id36">:ref:`logging-advanced-tutorial`</span></a>.</p>
<a name="user-content-logging-variable-data"></a>
<h3><a id="user-content-logging-variable-data" class="anchor" aria-hidden="true" href="#logging-variable-data"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Logging variable data</h3>
<p>To log variable data, use a format string for the event description message and
append the variable data as arguments. For example:</p>
<pre>import logging
logging.warning('%s before you %s', 'Look', 'leap!')
</pre>
<p>will display:</p>
<pre lang="none">WARNING:root:Look before you leap!
</pre>
<p>As you can see, merging of variable data into the event description message
uses the old, %-style of string formatting. This is for backwards
compatibility: the logging package pre-dates newer formatting options such as
<a href="#id37"><span id="user-content-id38">:meth:`str.format`</span></a> and <a href="#id39"><span id="user-content-id40">:class:`string.Template`</span></a>. These newer formatting
options <em>are</em> supported, but exploring them is outside the scope of this
tutorial: see <a href="#id41"><span id="user-content-id42">:ref:`formatting-styles`</span></a> for more information.</p>
<a name="user-content-changing-the-format-of-displayed-messages"></a>
<h3><a id="user-content-changing-the-format-of-displayed-messages" class="anchor" aria-hidden="true" href="#changing-the-format-of-displayed-messages"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Changing the format of displayed messages</h3>
<p>To change the format which is used to display messages, you need to
specify the format you want to use:</p>
<pre>import logging
logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.DEBUG)
logging.debug('This message should appear on the console')
logging.info('So should this')
logging.warning('And this, too')
</pre>
<p>which would print:</p>
<pre lang="none">DEBUG:This message should appear on the console
INFO:So should this
WARNING:And this, too
</pre>
<p>Notice that the 'root' which appeared in earlier examples has disappeared. For
a full set of things that can appear in format strings, you can refer to the
documentation for <a href="#id43"><span id="user-content-id44">:ref:`logrecord-attributes`</span></a>, but for simple usage, you just
need the <em>levelname</em> (severity), <em>message</em> (event description, including
variable data) and perhaps to display when the event occurred. This is
described in the next section.</p>
<a name="user-content-displaying-the-date-time-in-messages"></a>
<h3><a id="user-content-displaying-the-datetime-in-messages" class="anchor" aria-hidden="true" href="#displaying-the-datetime-in-messages"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Displaying the date/time in messages</h3>
<p>To display the date and time of an event, you would place '%(asctime)s' in
your format string:</p>
<pre>import logging
logging.basicConfig(format='%(asctime)s %(message)s')
logging.warning('is when this event was logged.')
</pre>
<p>which should print something like this:</p>
<pre lang="none">2010-12-12 11:41:42,612 is when this event was logged.
</pre>
<p>The default format for date/time display (shown above) is like ISO8601 or
<a href="http://tools.ietf.org/html/rfc3339.html" rel="nofollow">RFC 3339</a>. If you need more control over the formatting of the date/time, provide
a <em>datefmt</em> argument to <code>basicConfig</code>, as in this example:</p>
<pre>import logging
logging.basicConfig(format='%(asctime)s %(message)s', datefmt='%m/%d/%Y %I:%M:%S %p')
logging.warning('is when this event was logged.')
</pre>
<p>which would display something like this:</p>
<pre lang="none">12/12/2010 11:46:36 AM is when this event was logged.
</pre>
<p>The format of the <em>datefmt</em> argument is the same as supported by
<a href="#id45"><span id="user-content-id46">:func:`time.strftime`</span></a>.</p>
<a name="user-content-next-steps"></a>
<h3><a id="user-content-next-steps" class="anchor" aria-hidden="true" href="#next-steps"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Next Steps</h3>
<p>That concludes the basic tutorial. It should be enough to get you up and
running with logging. There's a lot more that the logging package offers, but
to get the best out of it, you'll need to invest a little more of your time in
reading the following sections. If you're ready for that, grab some of your
favourite beverage and carry on.</p>
<p>If your logging needs are simple, then use the above examples to incorporate
logging into your own scripts, and if you run into problems or don't
understand something, please post a question on the comp.lang.python Usenet
group (available at <a href="https://groups.google.com/forum/#!forum/comp.lang.python" rel="nofollow">https://groups.google.com/forum/#!forum/comp.lang.python</a>) and you
should receive help before too long.</p>
<p>Still here? You can carry on reading the next few sections, which provide a
slightly more advanced/in-depth tutorial than the basic one above. After that,
you can take a look at the <a href="#id47"><span id="user-content-id48">:ref:`logging-cookbook`</span></a>.</p>
<a name="user-content-advanced-logging-tutorial"></a>
<h2><a id="user-content-advanced-logging-tutorial" class="anchor" aria-hidden="true" href="#advanced-logging-tutorial"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Advanced Logging Tutorial</h2>
<p>The logging library takes a modular approach and offers several categories
of components: loggers, handlers, filters, and formatters.</p>
<ul>
<li>Loggers expose the interface that application code directly uses.</li>
<li>Handlers send the log records (created by loggers) to the appropriate
destination.</li>
<li>Filters provide a finer grained facility for determining which log records
to output.</li>
<li>Formatters specify the layout of log records in the final output.</li>
</ul>
<p>Log event information is passed between loggers, handlers, filters and
formatters in a <a href="#id49"><span id="user-content-id50">:class:`LogRecord`</span></a> instance.</p>
<p>Logging is performed by calling methods on instances of the <a href="#id51"><span id="user-content-id52">:class:`Logger`</span></a>
class (hereafter called <a href="#id53"><span id="user-content-id54">:dfn:`loggers`</span></a>). Each instance has a name, and they are
conceptually arranged in a namespace hierarchy using dots (periods) as
separators. For example, a logger named 'scan' is the parent of loggers
'scan.text', 'scan.html' and 'scan.pdf'. Logger names can be anything you want,
and indicate the area of an application in which a logged message originates.</p>
<p>A good convention to use when naming loggers is to use a module-level logger,
in each module which uses logging, named as follows:</p>
<pre>logger = logging.getLogger(__name__)
</pre>
<p>This means that logger names track the package/module hierarchy, and it's
intuitively obvious where events are logged just from the logger name.</p>
<p>The root of the hierarchy of loggers is called the root logger. That's the
logger used by the functions <a href="#id55"><span id="user-content-id56">:func:`debug`</span></a>, <a href="#id57"><span id="user-content-id58">:func:`info`</span></a>, <a href="#id59"><span id="user-content-id60">:func:`warning`</span></a>,
<a href="#id61"><span id="user-content-id62">:func:`error`</span></a> and <a href="#id63"><span id="user-content-id64">:func:`critical`</span></a>, which just call the same-named method of
the root logger. The functions and the methods have the same signatures. The
root logger's name is printed as 'root' in the logged output.</p>
<p>It is, of course, possible to log messages to different destinations. Support
is included in the package for writing log messages to files, HTTP GET/POST
locations, email via SMTP, generic sockets, queues, or OS-specific logging
mechanisms such as syslog or the Windows NT event log. Destinations are served
by <a href="#id65"><span id="user-content-id66">:dfn:`handler`</span></a> classes. You can create your own log destination class if
you have special requirements not met by any of the built-in handler classes.</p>
<p>By default, no destination is set for any logging messages. You can specify
a destination (such as console or file) by using <a href="#id67"><span id="user-content-id68">:func:`basicConfig`</span></a> as in the
tutorial examples. If you call the functions  <a href="#id69"><span id="user-content-id70">:func:`debug`</span></a>, <a href="#id71"><span id="user-content-id72">:func:`info`</span></a>,
<a href="#id73"><span id="user-content-id74">:func:`warning`</span></a>, <a href="#id75"><span id="user-content-id76">:func:`error`</span></a> and <a href="#id77"><span id="user-content-id78">:func:`critical`</span></a>, they will check to see
if no destination is set; and if one is not set, they will set a destination
of the console (<code>sys.stderr</code>) and a default format for the displayed
message before delegating to the root logger to do the actual message output.</p>
<p>The default format set by <a href="#id79"><span id="user-content-id80">:func:`basicConfig`</span></a> for messages is:</p>
<pre lang="none">severity:logger name:message
</pre>
<p>You can change this by passing a format string to <a href="#id81"><span id="user-content-id82">:func:`basicConfig`</span></a> with the
<em>format</em> keyword argument. For all options regarding how a format string is
constructed, see <a href="#id83"><span id="user-content-id84">:ref:`formatter-objects`</span></a>.</p>
<a name="user-content-logging-flow"></a>
<h3><a id="user-content-logging-flow" class="anchor" aria-hidden="true" href="#logging-flow"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Logging Flow</h3>
<p>The flow of log event information in loggers and handlers is illustrated in the
following diagram.</p>
<p><a target="_blank" rel="noopener noreferrer" href="/python/cpython/blob/master/Doc/howto/logging_flow.png"><img alt="logging_flow.png" src="/python/cpython/raw/master/Doc/howto/logging_flow.png" style="max-width:100%;"></a></p>
<a name="user-content-loggers"></a>
<h3><a id="user-content-loggers" class="anchor" aria-hidden="true" href="#loggers"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Loggers</h3>
<p><a href="#id85"><span id="user-content-id86">:class:`Logger`</span></a> objects have a threefold job.  First, they expose several
methods to application code so that applications can log messages at runtime.
Second, logger objects determine which log messages to act upon based upon
severity (the default filtering facility) or filter objects.  Third, logger
objects pass along relevant log messages to all interested log handlers.</p>
<p>The most widely used methods on logger objects fall into two categories:
configuration and message sending.</p>
<p>These are the most common configuration methods:</p>
<ul>
<li><a href="#id87"><span id="user-content-id88">:meth:`Logger.setLevel`</span></a> specifies the lowest-severity log message a logger
will handle, where debug is the lowest built-in severity level and critical
is the highest built-in severity.  For example, if the severity level is
INFO, the logger will handle only INFO, WARNING, ERROR, and CRITICAL messages
and will ignore DEBUG messages.</li>
<li><a href="#id89"><span id="user-content-id90">:meth:`Logger.addHandler`</span></a> and <a href="#id91"><span id="user-content-id92">:meth:`Logger.removeHandler`</span></a> add and remove
handler objects from the logger object.  Handlers are covered in more detail
in <a href="#id93"><span id="user-content-id94">:ref:`handler-basic`</span></a>.</li>
<li><a href="#id95"><span id="user-content-id96">:meth:`Logger.addFilter`</span></a> and <a href="#id97"><span id="user-content-id98">:meth:`Logger.removeFilter`</span></a> add and remove filter
objects from the logger object.  Filters are covered in more detail in
<a href="#id99"><span id="user-content-id100">:ref:`filter`</span></a>.</li>
</ul>
<p>You don't need to always call these methods on every logger you create. See the
last two paragraphs in this section.</p>
<p>With the logger object configured, the following methods create log messages:</p>
<ul>
<li><a href="#id101"><span id="user-content-id102">:meth:`Logger.debug`</span></a>, <a href="#id103"><span id="user-content-id104">:meth:`Logger.info`</span></a>, <a href="#id105"><span id="user-content-id106">:meth:`Logger.warning`</span></a>,
<a href="#id107"><span id="user-content-id108">:meth:`Logger.error`</span></a>, and <a href="#id109"><span id="user-content-id110">:meth:`Logger.critical`</span></a> all create log records with
a message and a level that corresponds to their respective method names. The
message is actually a format string, which may contain the standard string
substitution syntax of <code>%s</code>, <code>%d</code>, <code>%f</code>, and so on.  The
rest of their arguments is a list of objects that correspond with the
substitution fields in the message.  With regard to <code>**kwargs</code>, the
logging methods care only about a keyword of <code>exc_info</code> and use it to
determine whether to log exception information.</li>
<li><a href="#id111"><span id="user-content-id112">:meth:`Logger.exception`</span></a> creates a log message similar to
<a href="#id113"><span id="user-content-id114">:meth:`Logger.error`</span></a>.  The difference is that <a href="#id115"><span id="user-content-id116">:meth:`Logger.exception`</span></a> dumps a
stack trace along with it.  Call this method only from an exception handler.</li>
<li><a href="#id117"><span id="user-content-id118">:meth:`Logger.log`</span></a> takes a log level as an explicit argument.  This is a
little more verbose for logging messages than using the log level convenience
methods listed above, but this is how to log at custom log levels.</li>
</ul>
<p><a href="#id119"><span id="user-content-id120">:func:`getLogger`</span></a> returns a reference to a logger instance with the specified
name if it is provided, or <code>root</code> if not.  The names are period-separated
hierarchical structures.  Multiple calls to <a href="#id121"><span id="user-content-id122">:func:`getLogger`</span></a> with the same name
will return a reference to the same logger object.  Loggers that are further
down in the hierarchical list are children of loggers higher up in the list.
For example, given a logger with a name of <code>foo</code>, loggers with names of
<code>foo.bar</code>, <code>foo.bar.baz</code>, and <code>foo.bam</code> are all descendants of <code>foo</code>.</p>
<p>Loggers have a concept of <em>effective level</em>. If a level is not explicitly set
on a logger, the level of its parent is used instead as its effective level.
If the parent has no explicit level set, <em>its</em> parent is examined, and so on -
all ancestors are searched until an explicitly set level is found. The root
logger always has an explicit level set (<code>WARNING</code> by default). When deciding
whether to process an event, the effective level of the logger is used to
determine whether the event is passed to the logger's handlers.</p>
<p>Child loggers propagate messages up to the handlers associated with their
ancestor loggers. Because of this, it is unnecessary to define and configure
handlers for all the loggers an application uses. It is sufficient to
configure handlers for a top-level logger and create child loggers as needed.
(You can, however, turn off propagation by setting the <em>propagate</em>
attribute of a logger to <code>False</code>.)</p>
<a name="user-content-handlers"></a>
<h3><a id="user-content-handlers" class="anchor" aria-hidden="true" href="#handlers"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Handlers</h3>
<p><a href="#id123"><span id="user-content-id124">:class:`~logging.Handler`</span></a> objects are responsible for dispatching the
appropriate log messages (based on the log messages' severity) to the handler's
specified destination.  <a href="#id125"><span id="user-content-id126">:class:`Logger`</span></a> objects can add zero or more handler
objects to themselves with an <a href="#id127"><span id="user-content-id128">:meth:`~Logger.addHandler`</span></a> method.  As an example
scenario, an application may want to send all log messages to a log file, all
log messages of error or higher to stdout, and all messages of critical to an
email address. This scenario requires three individual handlers where each
handler is responsible for sending messages of a specific severity to a specific
location.</p>
<p>The standard library includes quite a few handler types (see
<a href="#id129"><span id="user-content-id130">:ref:`useful-handlers`</span></a>); the tutorials use mainly <a href="#id131"><span id="user-content-id132">:class:`StreamHandler`</span></a> and
<a href="#id133"><span id="user-content-id134">:class:`FileHandler`</span></a> in its examples.</p>
<p>There are very few methods in a handler for application developers to concern
themselves with.  The only handler methods that seem relevant for application
developers who are using the built-in handler objects (that is, not creating
custom handlers) are the following configuration methods:</p>
<ul>
<li>The <a href="#id135"><span id="user-content-id136">:meth:`~Handler.setLevel`</span></a> method, just as in logger objects, specifies the
lowest severity that will be dispatched to the appropriate destination.  Why
are there two <a href="#id137"><span id="user-content-id138">:func:`setLevel`</span></a> methods?  The level set in the logger
determines which severity of messages it will pass to its handlers.  The level
set in each handler determines which messages that handler will send on.</li>
<li><a href="#id139"><span id="user-content-id140">:meth:`~Handler.setFormatter`</span></a> selects a Formatter object for this handler to
use.</li>
<li><a href="#id141"><span id="user-content-id142">:meth:`~Handler.addFilter`</span></a> and <a href="#id143"><span id="user-content-id144">:meth:`~Handler.removeFilter`</span></a> respectively
configure and deconfigure filter objects on handlers.</li>
</ul>
<p>Application code should not directly instantiate and use instances of
<a href="#id145"><span id="user-content-id146">:class:`Handler`</span></a>.  Instead, the <a href="#id147"><span id="user-content-id148">:class:`Handler`</span></a> class is a base class that
defines the interface that all handlers should have and establishes some
default behavior that child classes can use (or override).</p>
<a name="user-content-formatters"></a>
<h3><a id="user-content-formatters" class="anchor" aria-hidden="true" href="#formatters"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Formatters</h3>
<p>Formatter objects configure the final order, structure, and contents of the log
message.  Unlike the base <a href="#id149"><span id="user-content-id150">:class:`logging.Handler`</span></a> class, application code may
instantiate formatter classes, although you could likely subclass the formatter
if your application needs special behavior.  The constructor takes three
optional arguments -- a message format string, a date format string and a style
indicator.</p>
<pre>.. method:: logging.Formatter.__init__(fmt=None, datefmt=None, style='%')

</pre>
<p>If there is no message format string, the default is to use the
raw message.  If there is no date format string, the default date format is:</p>
<pre lang="none">%Y-%m-%d %H:%M:%S
</pre>
<p>with the milliseconds tacked on at the end. The <code>style</code> is one of %, '{'
or '$'. If one of these is not specified, then '%' will be used.</p>
<p>If the <code>style</code> is '%', the message format string uses
<code>%(&lt;dictionary key&gt;)s</code> styled string substitution; the possible keys are
documented in <a href="#id151"><span id="user-content-id152">:ref:`logrecord-attributes`</span></a>. If the style is '{', the message
format string is assumed to be compatible with <a href="#id153"><span id="user-content-id154">:meth:`str.format`</span></a> (using
keyword arguments), while if the style is '$' then the message format string
should conform to what is expected by <a href="#id155"><span id="user-content-id156">:meth:`string.Template.substitute`</span></a>.</p>
<pre>.. versionchanged:: 3.2
   Added the ``style`` parameter.

</pre>
<p>The following message format string will log the time in a human-readable
format, the severity of the message, and the contents of the message, in that
order:</p>
<pre>'%(asctime)s - %(levelname)s - %(message)s'
</pre>
<p>Formatters use a user-configurable function to convert the creation time of a
record to a tuple. By default, <a href="#id157"><span id="user-content-id158">:func:`time.localtime`</span></a> is used; to change this
for a particular formatter instance, set the <code>converter</code> attribute of the
instance to a function with the same signature as <a href="#id159"><span id="user-content-id160">:func:`time.localtime`</span></a> or
<a href="#id161"><span id="user-content-id162">:func:`time.gmtime`</span></a>. To change it for all formatters, for example if you want
all logging times to be shown in GMT, set the <code>converter</code> attribute in the
Formatter class (to <code>time.gmtime</code> for GMT display).</p>
<a name="user-content-configuring-logging"></a>
<h3><a id="user-content-configuring-logging" class="anchor" aria-hidden="true" href="#configuring-logging"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Configuring Logging</h3>
<pre>.. currentmodule:: logging.config

</pre>
<p>Programmers can configure logging in three ways:</p>
<ol>
<li>Creating loggers, handlers, and formatters explicitly using Python
code that calls the configuration methods listed above.</li>
<li>Creating a logging config file and reading it using the <a href="#id163"><span id="user-content-id164">:func:`fileConfig`</span></a>
function.</li>
<li>Creating a dictionary of configuration information and passing it
to the <a href="#id165"><span id="user-content-id166">:func:`dictConfig`</span></a> function.</li>
</ol>
<p>For the reference documentation on the last two options, see
<a href="#id167"><span id="user-content-id168">:ref:`logging-config-api`</span></a>.  The following example configures a very simple
logger, a console handler, and a simple formatter using Python code:</p>
<pre>import logging

# create logger
logger = logging.getLogger('simple_example')
logger.setLevel(logging.DEBUG)

# create console handler and set level to debug
ch = logging.StreamHandler()
ch.setLevel(logging.DEBUG)

# create formatter
formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')

# add formatter to ch
ch.setFormatter(formatter)

# add ch to logger
logger.addHandler(ch)

# 'application' code
logger.debug('debug message')
logger.info('info message')
logger.warning('warn message')
logger.error('error message')
logger.critical('critical message')
</pre>
<p>Running this module from the command line produces the following output:</p>
<pre lang="shell-session">$ python simple_logging_module.py
2005-03-19 15:10:26,618 - simple_example - DEBUG - debug message
2005-03-19 15:10:26,620 - simple_example - INFO - info message
2005-03-19 15:10:26,695 - simple_example - WARNING - warn message
2005-03-19 15:10:26,697 - simple_example - ERROR - error message
2005-03-19 15:10:26,773 - simple_example - CRITICAL - critical message
</pre>
<p>The following Python module creates a logger, handler, and formatter nearly
identical to those in the example listed above, with the only difference being
the names of the objects:</p>
<pre>import logging
import logging.config

logging.config.fileConfig('logging.conf')

# create logger
logger = logging.getLogger('simpleExample')

# 'application' code
logger.debug('debug message')
logger.info('info message')
logger.warning('warn message')
logger.error('error message')
logger.critical('critical message')
</pre>
<p>Here is the logging.conf file:</p>
<div class="highlight highlight-source-ini"><pre><span class="pl-en">[loggers]</span>
<span class="pl-k">keys</span>=root,simpleExample

<span class="pl-en">[handlers]</span>
<span class="pl-k">keys</span>=consoleHandler

<span class="pl-en">[formatters]</span>
<span class="pl-k">keys</span>=simpleFormatter

<span class="pl-en">[logger_root]</span>
<span class="pl-k">level</span>=DEBUG
<span class="pl-k">handlers</span>=consoleHandler

<span class="pl-en">[logger_simpleExample]</span>
<span class="pl-k">level</span>=DEBUG
<span class="pl-k">handlers</span>=consoleHandler
<span class="pl-k">qualname</span>=simpleExample
<span class="pl-k">propagate</span>=0

<span class="pl-en">[handler_consoleHandler]</span>
<span class="pl-k">class</span>=StreamHandler
<span class="pl-k">level</span>=DEBUG
<span class="pl-k">formatter</span>=simpleFormatter
<span class="pl-k">args</span>=(sys.stdout,)

<span class="pl-en">[formatter_simpleFormatter]</span>
<span class="pl-k">format</span>=%(asctime)s - %(name)s - %(levelname)s - %(message)s
<span class="pl-k">datefmt</span>=</pre></div>
<p>The output is nearly identical to that of the non-config-file-based example:</p>
<pre lang="shell-session">$ python simple_logging_config.py
2005-03-19 15:38:55,977 - simpleExample - DEBUG - debug message
2005-03-19 15:38:55,979 - simpleExample - INFO - info message
2005-03-19 15:38:56,054 - simpleExample - WARNING - warn message
2005-03-19 15:38:56,055 - simpleExample - ERROR - error message
2005-03-19 15:38:56,130 - simpleExample - CRITICAL - critical message
</pre>
<p>You can see that the config file approach has a few advantages over the Python
code approach, mainly separation of configuration and code and the ability of
noncoders to easily modify the logging properties.</p>
<div>
<p>Warning</p>
<p>The <a href="#id169"><span id="user-content-id170">:func:`fileConfig`</span></a> function takes a default parameter,
<code>disable_existing_loggers</code>, which defaults to <code>True</code> for reasons of
backward compatibility. This may or may not be what you want, since it
will cause any non-root loggers existing before the <a href="#id171"><span id="user-content-id172">:func:`fileConfig`</span></a>
call to be disabled unless they (or an ancestor) are explicitly named in
the configuration. Please refer to the reference documentation for more
information, and specify <code>False</code> for this parameter if you wish.</p>
<p>The dictionary passed to <a href="#id173"><span id="user-content-id174">:func:`dictConfig`</span></a> can also specify a Boolean
value with key <code>disable_existing_loggers</code>, which if not specified
explicitly in the dictionary also defaults to being interpreted as
<code>True</code>. This leads to the logger-disabling behaviour described above,
which may not be what you want - in which case, provide the key
explicitly with a value of <code>False</code>.</p>
</div>
<pre>.. currentmodule:: logging

</pre>
<p>Note that the class names referenced in config files need to be either relative
to the logging module, or absolute values which can be resolved using normal
import mechanisms. Thus, you could use either
<a href="#id175"><span id="user-content-id176">:class:`~logging.handlers.WatchedFileHandler`</span></a> (relative to the logging module) or
<code>mypackage.mymodule.MyHandler</code> (for a class defined in package <code>mypackage</code>
and module <code>mymodule</code>, where <code>mypackage</code> is available on the Python import
path).</p>
<p>In Python 3.2, a new means of configuring logging has been introduced, using
dictionaries to hold configuration information. This provides a superset of the
functionality of the config-file-based approach outlined above, and is the
recommended configuration method for new applications and deployments. Because
a Python dictionary is used to hold configuration information, and since you
can populate that dictionary using different means, you have more options for
configuration. For example, you can use a configuration file in JSON format,
or, if you have access to YAML processing functionality, a file in YAML
format, to populate the configuration dictionary. Or, of course, you can
construct the dictionary in Python code, receive it in pickled form over a
socket, or use whatever approach makes sense for your application.</p>
<p>Here's an example of the same configuration as above, in YAML format for
the new dictionary-based approach:</p>
<div class="highlight highlight-source-yaml"><pre><span class="pl-ent">version</span>: <span class="pl-c1">1</span>
<span class="pl-ent">formatters</span>:
  <span class="pl-ent">simple</span>:
    <span class="pl-ent">format</span>: <span class="pl-s"><span class="pl-pds">'</span>%(asctime)s - %(name)s - %(levelname)s - %(message)s<span class="pl-pds">'</span></span>
<span class="pl-ent">handlers</span>:
  <span class="pl-ent">console</span>:
    <span class="pl-ent">class</span>: <span class="pl-s">logging.StreamHandler</span>
    <span class="pl-ent">level</span>: <span class="pl-s">DEBUG</span>
    <span class="pl-ent">formatter</span>: <span class="pl-s">simple</span>
    <span class="pl-ent">stream</span>: <span class="pl-s">ext://sys.stdout</span>
<span class="pl-ent">loggers</span>:
  <span class="pl-ent">simpleExample</span>:
    <span class="pl-ent">level</span>: <span class="pl-s">DEBUG</span>
    <span class="pl-ent">handlers</span>: <span class="pl-s">[console]</span>
    <span class="pl-ent">propagate</span>: <span class="pl-s">no</span>
<span class="pl-ent">root</span>:
  <span class="pl-ent">level</span>: <span class="pl-s">DEBUG</span>
  <span class="pl-ent">handlers</span>: <span class="pl-s">[console]</span></pre></div>
<p>For more information about logging using a dictionary, see
<a href="#id177"><span id="user-content-id178">:ref:`logging-config-api`</span></a>.</p>
<a name="user-content-what-happens-if-no-configuration-is-provided"></a>
<h3><a id="user-content-what-happens-if-no-configuration-is-provided" class="anchor" aria-hidden="true" href="#what-happens-if-no-configuration-is-provided"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>What happens if no configuration is provided</h3>
<p>If no logging configuration is provided, it is possible to have a situation
where a logging event needs to be output, but no handlers can be found to
output the event. The behaviour of the logging package in these
circumstances is dependent on the Python version.</p>
<p>For versions of Python prior to 3.2, the behaviour is as follows:</p>
<ul>
<li>If <em>logging.raiseExceptions</em> is <code>False</code> (production mode), the event is
silently dropped.</li>
<li>If <em>logging.raiseExceptions</em> is <code>True</code> (development mode), a message
'No handlers could be found for logger X.Y.Z' is printed once.</li>
</ul>
<p>In Python 3.2 and later, the behaviour is as follows:</p>
<ul>
<li>The event is output using a 'handler of last resort', stored in
<code>logging.lastResort</code>. This internal handler is not associated with any
logger, and acts like a <a href="#id179"><span id="user-content-id180">:class:`~logging.StreamHandler`</span></a> which writes the
event description message to the current value of <code>sys.stderr</code> (therefore
respecting any redirections which may be in effect). No formatting is
done on the message - just the bare event description message is printed.
The handler's level is set to <code>WARNING</code>, so all events at this and
greater severities will be output.</li>
</ul>
<p>To obtain the pre-3.2 behaviour, <code>logging.lastResort</code> can be set to <code>None</code>.</p>
<a name="user-content-configuring-logging-for-a-library"></a>
<h3><a id="user-content-configuring-logging-for-a-library" class="anchor" aria-hidden="true" href="#configuring-logging-for-a-library"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Configuring Logging for a Library</h3>
<p>When developing a library which uses logging, you should take care to
document how the library uses logging - for example, the names of loggers
used. Some consideration also needs to be given to its logging configuration.
If the using application does not use logging, and library code makes logging
calls, then (as described in the previous section) events of severity
<code>WARNING</code> and greater will be printed to <code>sys.stderr</code>. This is regarded as
the best default behaviour.</p>
<p>If for some reason you <em>don't</em> want these messages printed in the absence of
any logging configuration, you can attach a do-nothing handler to the top-level
logger for your library. This avoids the message being printed, since a handler
will always be found for the library's events: it just doesn't produce any
output. If the library user configures logging for application use, presumably
that configuration will add some handlers, and if levels are suitably
configured then logging calls made in library code will send output to those
handlers, as normal.</p>
<p>A do-nothing handler is included in the logging package:
<a href="#id181"><span id="user-content-id182">:class:`~logging.NullHandler`</span></a> (since Python 3.1). An instance of this handler
could be added to the top-level logger of the logging namespace used by the
library (<em>if</em> you want to prevent your library's logged events being output to
<code>sys.stderr</code> in the absence of logging configuration). If all logging by a
library <em>foo</em> is done using loggers with names matching 'foo.x', 'foo.x.y',
etc. then the code:</p>
<pre>import logging
logging.getLogger('foo').addHandler(logging.NullHandler())
</pre>
<p>should have the desired effect. If an organisation produces a number of
libraries, then the logger name specified can be 'orgname.foo' rather than
just 'foo'.</p>
<div>
<p>Note</p>
<p>It is strongly advised that you <em>do not add any handlers other
than</em> <a href="#id183"><span id="user-content-id184">:class:`~logging.NullHandler`</span></a> <em>to your library's loggers</em>. This is
because the configuration of handlers is the prerogative of the application
developer who uses your library. The application developer knows their
target audience and what handlers are most appropriate for their
application: if you add handlers 'under the hood', you might well interfere
with their ability to carry out unit tests and deliver logs which suit their
requirements.</p>
</div>
<a name="user-content-logging-levels"></a>
<h2><a id="user-content-logging-levels" class="anchor" aria-hidden="true" href="#logging-levels"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Logging Levels</h2>
<p>The numeric values of logging levels are given in the following table. These are
primarily of interest if you want to define your own levels, and need them to
have specific values relative to the predefined levels. If you define a level
with the same numeric value, it overwrites the predefined value; the predefined
name is lost.</p>
<table>




<thead valign="bottom">
<tr><th>Level</th>
<th>Numeric value</th>
</tr>
</thead>
<tbody valign="top">
<tr><td><code>CRITICAL</code></td>
<td>50</td>
</tr>
<tr><td><code>ERROR</code></td>
<td>40</td>
</tr>
<tr><td><code>WARNING</code></td>
<td>30</td>
</tr>
<tr><td><code>INFO</code></td>
<td>20</td>
</tr>
<tr><td><code>DEBUG</code></td>
<td>10</td>
</tr>
<tr><td><code>NOTSET</code></td>
<td>0</td>
</tr>
</tbody>
</table>
<p>Levels can also be associated with loggers, being set either by the developer or
through loading a saved logging configuration. When a logging method is called
on a logger, the logger compares its own level with the level associated with
the method call. If the logger's level is higher than the method call's, no
logging message is actually generated. This is the basic mechanism controlling
the verbosity of logging output.</p>
<p>Logging messages are encoded as instances of the <a href="#id185"><span id="user-content-id186">:class:`~logging.LogRecord`</span></a>
class. When a logger decides to actually log an event, a
<a href="#id187"><span id="user-content-id188">:class:`~logging.LogRecord`</span></a> instance is created from the logging message.</p>
<p>Logging messages are subjected to a dispatch mechanism through the use of
<a href="#id189"><span id="user-content-id190">:dfn:`handlers`</span></a>, which are instances of subclasses of the <a href="#id191"><span id="user-content-id192">:class:`Handler`</span></a>
class. Handlers are responsible for ensuring that a logged message (in the form
of a <a href="#id193"><span id="user-content-id194">:class:`LogRecord`</span></a>) ends up in a particular location (or set of locations)
which is useful for the target audience for that message (such as end users,
support desk staff, system administrators, developers). Handlers are passed
<a href="#id195"><span id="user-content-id196">:class:`LogRecord`</span></a> instances intended for particular destinations. Each logger
can have zero, one or more handlers associated with it (via the
<a href="#id197"><span id="user-content-id198">:meth:`~Logger.addHandler`</span></a> method of <a href="#id199"><span id="user-content-id200">:class:`Logger`</span></a>). In addition to any
handlers directly associated with a logger, <em>all handlers associated with all
ancestors of the logger</em> are called to dispatch the message (unless the
<em>propagate</em> flag for a logger is set to a false value, at which point the
passing to ancestor handlers stops).</p>
<p>Just as for loggers, handlers can have levels associated with them. A handler's
level acts as a filter in the same way as a logger's level does. If a handler
decides to actually dispatch an event, the <a href="#id201"><span id="user-content-id202">:meth:`~Handler.emit`</span></a> method is used
to send the message to its destination. Most user-defined subclasses of
<a href="#id203"><span id="user-content-id204">:class:`Handler`</span></a> will need to override this <a href="#id205"><span id="user-content-id206">:meth:`~Handler.emit`</span></a>.</p>
<a name="user-content-id207"></a>
<h3><a id="user-content-custom-levels" class="anchor" aria-hidden="true" href="#custom-levels"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Custom Levels</h3>
<p>Defining your own levels is possible, but should not be necessary, as the
existing levels have been chosen on the basis of practical experience.
However, if you are convinced that you need custom levels, great care should
be exercised when doing this, and it is possibly <em>a very bad idea to define
custom levels if you are developing a library</em>. That's because if multiple
library authors all define their own custom levels, there is a chance that
the logging output from such multiple libraries used together will be
difficult for the using developer to control and/or interpret, because a
given numeric value might mean different things for different libraries.</p>
<a name="user-content-id208"></a>
<h2><a id="user-content-useful-handlers" class="anchor" aria-hidden="true" href="#useful-handlers"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Useful Handlers</h2>
<p>In addition to the base <a href="#id209"><span id="user-content-id210">:class:`Handler`</span></a> class, many useful subclasses are
provided:</p>
<ol>
<li><a href="#id211"><span id="user-content-id212">:class:`StreamHandler`</span></a> instances send messages to streams (file-like
objects).</li>
<li><a href="#id213"><span id="user-content-id214">:class:`FileHandler`</span></a> instances send messages to disk files.</li>
<li><a href="#id215"><span id="user-content-id216">:class:`~handlers.BaseRotatingHandler`</span></a> is the base class for handlers that
rotate log files at a certain point. It is not meant to be  instantiated
directly. Instead, use <a href="#id217"><span id="user-content-id218">:class:`~handlers.RotatingFileHandler`</span></a> or
<a href="#id219"><span id="user-content-id220">:class:`~handlers.TimedRotatingFileHandler`</span></a>.</li>
<li><a href="#id221"><span id="user-content-id222">:class:`~handlers.RotatingFileHandler`</span></a> instances send messages to disk
files, with support for maximum log file sizes and log file rotation.</li>
<li><a href="#id223"><span id="user-content-id224">:class:`~handlers.TimedRotatingFileHandler`</span></a> instances send messages to
disk files, rotating the log file at certain timed intervals.</li>
<li><a href="#id225"><span id="user-content-id226">:class:`~handlers.SocketHandler`</span></a> instances send messages to TCP/IP
sockets. Since 3.4, Unix domain sockets are also supported.</li>
<li><a href="#id227"><span id="user-content-id228">:class:`~handlers.DatagramHandler`</span></a> instances send messages to UDP
sockets. Since 3.4, Unix domain sockets are also supported.</li>
<li><a href="#id229"><span id="user-content-id230">:class:`~handlers.SMTPHandler`</span></a> instances send messages to a designated
email address.</li>
<li><a href="#id231"><span id="user-content-id232">:class:`~handlers.SysLogHandler`</span></a> instances send messages to a Unix
syslog daemon, possibly on a remote machine.</li>
<li><a href="#id233"><span id="user-content-id234">:class:`~handlers.NTEventLogHandler`</span></a> instances send messages to a
Windows NT/2000/XP event log.</li>
<li><a href="#id235"><span id="user-content-id236">:class:`~handlers.MemoryHandler`</span></a> instances send messages to a buffer
in memory, which is flushed whenever specific criteria are met.</li>
<li><a href="#id237"><span id="user-content-id238">:class:`~handlers.HTTPHandler`</span></a> instances send messages to an HTTP
server using either <code>GET</code> or <code>POST</code> semantics.</li>
<li><a href="#id239"><span id="user-content-id240">:class:`~handlers.WatchedFileHandler`</span></a> instances watch the file they are
logging to. If the file changes, it is closed and reopened using the file
name. This handler is only useful on Unix-like systems; Windows does not
support the underlying mechanism used.</li>
<li><a href="#id241"><span id="user-content-id242">:class:`~handlers.QueueHandler`</span></a> instances send messages to a queue, such as
those implemented in the <a href="#id243"><span id="user-content-id244">:mod:`queue`</span></a> or <a href="#id245"><span id="user-content-id246">:mod:`multiprocessing`</span></a> modules.</li>
<li><a href="#id247"><span id="user-content-id248">:class:`NullHandler`</span></a> instances do nothing with error messages. They are used
by library developers who want to use logging, but want to avoid the 'No
handlers could be found for logger XXX' message which can be displayed if
the library user has not configured logging. See <a href="#id249"><span id="user-content-id250">:ref:`library-config`</span></a> for
more information.</li>
</ol>
<pre>.. versionadded:: 3.1
   The :class:`NullHandler` class.

</pre>
<pre>.. versionadded:: 3.2
   The :class:`~handlers.QueueHandler` class.

</pre>
<p>The <a href="#id251"><span id="user-content-id252">:class:`NullHandler`</span></a>, <a href="#id253"><span id="user-content-id254">:class:`StreamHandler`</span></a> and <a href="#id255"><span id="user-content-id256">:class:`FileHandler`</span></a>
classes are defined in the core logging package. The other handlers are
defined in a sub-module, <a href="#id257"><span id="user-content-id258">:mod:`logging.handlers`</span></a>. (There is also another
sub-module, <a href="#id259"><span id="user-content-id260">:mod:`logging.config`</span></a>, for configuration functionality.)</p>
<p>Logged messages are formatted for presentation through instances of the
<a href="#id261"><span id="user-content-id262">:class:`Formatter`</span></a> class. They are initialized with a format string suitable for
use with the % operator and a dictionary.</p>
<p>For formatting multiple messages in a batch, instances of
<a href="#id263"><span id="user-content-id264">:class:`~handlers.BufferingFormatter`</span></a> can be used. In addition to the format
string (which is applied to each message in the batch), there is provision for
header and trailer format strings.</p>
<p>When filtering based on logger level and/or handler level is not enough,
instances of <a href="#id265"><span id="user-content-id266">:class:`Filter`</span></a> can be added to both <a href="#id267"><span id="user-content-id268">:class:`Logger`</span></a> and
<a href="#id269"><span id="user-content-id270">:class:`Handler`</span></a> instances (through their <a href="#id271"><span id="user-content-id272">:meth:`~Handler.addFilter`</span></a> method).
Before deciding to process a message further, both loggers and handlers consult
all their filters for permission. If any filter returns a false value, the
message is not processed further.</p>
<p>The basic <a href="#id273"><span id="user-content-id274">:class:`Filter`</span></a> functionality allows filtering by specific logger
name. If this feature is used, messages sent to the named logger and its
children are allowed through the filter, and all others dropped.</p>
<a name="user-content-exceptions-raised-during-logging"></a>
<h2><a id="user-content-exceptions-raised-during-logging" class="anchor" aria-hidden="true" href="#exceptions-raised-during-logging"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Exceptions raised during logging</h2>
<p>The logging package is designed to swallow exceptions which occur while logging
in production. This is so that errors which occur while handling logging events
- such as logging misconfiguration, network or other similar errors - do not
cause the application using logging to terminate prematurely.</p>
<p><a href="#id275"><span id="user-content-id276">:class:`SystemExit`</span></a> and <a href="#id277"><span id="user-content-id278">:class:`KeyboardInterrupt`</span></a> exceptions are never
swallowed. Other exceptions which occur during the <a href="#id279"><span id="user-content-id280">:meth:`~Handler.emit`</span></a> method
of a <a href="#id281"><span id="user-content-id282">:class:`Handler`</span></a> subclass are passed to its <a href="#id283"><span id="user-content-id284">:meth:`~Handler.handleError`</span></a>
method.</p>
<p>The default implementation of <a href="#id285"><span id="user-content-id286">:meth:`~Handler.handleError`</span></a> in <a href="#id287"><span id="user-content-id288">:class:`Handler`</span></a>
checks to see if a module-level variable, <a href="#id289"><span id="user-content-id290">:data:`raiseExceptions`</span></a>, is set. If
set, a traceback is printed to <a href="#id291"><span id="user-content-id292">:data:`sys.stderr`</span></a>. If not set, the exception is
swallowed.</p>
<div>
<p>Note</p>
<p>The default value of <a href="#id293"><span id="user-content-id294">:data:`raiseExceptions`</span></a> is <code>True</code>. This is
because during development, you typically want to be notified of any
exceptions that occur. It's advised that you set <a href="#id295"><span id="user-content-id296">:data:`raiseExceptions`</span></a> to
<code>False</code> for production usage.</p>
</div>
<pre>.. currentmodule:: logging

</pre>
<a name="user-content-using-arbitrary-objects-as-messages"></a>
<h2><a id="user-content-using-arbitrary-objects-as-messages" class="anchor" aria-hidden="true" href="#using-arbitrary-objects-as-messages"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Using arbitrary objects as messages</h2>
<p>In the preceding sections and examples, it has been assumed that the message
passed when logging the event is a string. However, this is not the only
possibility. You can pass an arbitrary object as a message, and its
<a href="#id297"><span id="user-content-id298">:meth:`~object.__str__`</span></a> method will be called when the logging system needs to
convert it to a string representation. In fact, if you want to, you can avoid
computing a string representation altogether - for example, the
<a href="#id299"><span id="user-content-id300">:class:`~handlers.SocketHandler`</span></a> emits an event by pickling it and sending it
over the wire.</p>
<a name="user-content-optimization"></a>
<h2><a id="user-content-optimization" class="anchor" aria-hidden="true" href="#optimization"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Optimization</h2>
<p>Formatting of message arguments is deferred until it cannot be avoided.
However, computing the arguments passed to the logging method can also be
expensive, and you may want to avoid doing it if the logger will just throw
away your event. To decide what to do, you can call the
<a href="#id301"><span id="user-content-id302">:meth:`~Logger.isEnabledFor`</span></a> method which takes a level argument and returns
true if the event would be created by the Logger for that level of call.
You can write code like this:</p>
<pre>if logger.isEnabledFor(logging.DEBUG):
    logger.debug('Message with %s, %s', expensive_func1(),
                                        expensive_func2())
</pre>
<p>so that if the logger's threshold is set above <code>DEBUG</code>, the calls to
<a href="#id303"><span id="user-content-id304">:func:`expensive_func1`</span></a> and <a href="#id305"><span id="user-content-id306">:func:`expensive_func2`</span></a> are never made.</p>
<div>
<p>Note</p>
<p>In some cases, <a href="#id307"><span id="user-content-id308">:meth:`~Logger.isEnabledFor`</span></a> can itself be more
expensive than you'd like (e.g. for deeply nested loggers where an explicit
level is only set high up in the logger hierarchy). In such cases (or if you
want to avoid calling a method in tight loops), you can cache the result of a
call to <a href="#id309"><span id="user-content-id310">:meth:`~Logger.isEnabledFor`</span></a> in a local or instance variable, and use
that instead of calling the method each time. Such a cached value would only
need to be recomputed when the logging configuration changes dynamically
while the application is running (which is not all that common).</p>
</div>
<p>There are other optimizations which can be made for specific applications which
need more precise control over what logging information is collected. Here's a
list of things you can do to avoid processing during logging which you don't
need:</p>
<table>




<thead valign="bottom">
<tr><th>What you don't want to collect</th>
<th>How to avoid collecting it</th>
</tr>
</thead>
<tbody valign="top">
<tr><td>Information about where calls were made from.</td>
<td>Set <code>logging._srcfile</code> to <code>None</code>.
This avoids calling
<a href="#id311"><span id="user-content-id312">:func:`sys._getframe`</span></a>, which may help
to speed up your code in environments
like PyPy (which can't speed up code
that uses <a href="#id313"><span id="user-content-id314">:func:`sys._getframe`</span></a>), if
and when PyPy supports Python 3.x.</td>
</tr>
<tr><td>Threading information.</td>
<td>Set <code>logging.logThreads</code> to <code>0</code>.</td>
</tr>
<tr><td>Process information.</td>
<td>Set <code>logging.logProcesses</code> to <code>0</code>.</td>
</tr>
</tbody>
</table>
<p>Also note that the core logging module only includes the basic handlers. If
you don't import <a href="#id315"><span id="user-content-id316">:mod:`logging.handlers`</span></a> and <a href="#id317"><span id="user-content-id318">:mod:`logging.config`</span></a>, they won't
take up any memory.</p>
<pre>.. seealso::

   Module :mod:`logging`
      API reference for the logging module.

   Module :mod:`logging.config`
      Configuration API for the logging module.

   Module :mod:`logging.handlers`
      Useful handlers included with the logging module.

   :ref:`A logging cookbook &lt;logging-cookbook&gt;`
</pre>

</article>
  </div>

    </div>

  

  <details class="details-reset details-overlay details-overlay-dark">
    <summary data-hotkey="l" aria-label="Jump to line"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast linejump" aria-label="Jump to line">
      <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-jump-to-line-form Box-body d-flex" action="" accept-charset="UTF-8" method="get"><input name="utf8" type="hidden" value="&#x2713;" />
        <input class="form-control flex-auto mr-3 linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
        <button type="submit" class="btn" data-close-dialog>Go</button>
</form>    </details-dialog>
  </details>



  </div>
  <div class="modal-backdrop js-touch-events"></div>
</div>

    </main>
  </div>
  

  </div>

        
<div class="footer container-lg px-3" role="contentinfo">
  <div class="position-relative d-flex flex-justify-between pt-6 pb-2 mt-6 f6 text-gray border-top border-gray-light ">
    <ul class="list-style-none d-flex flex-wrap ">
      <li class="mr-3">&copy; 2019 <span title="0.28443s from unicorn-798999d7cf-s59bg">GitHub</span>, Inc.</li>
        <li class="mr-3"><a data-ga-click="Footer, go to terms, text:terms" href="https://github.com/site/terms">Terms</a></li>
        <li class="mr-3"><a data-ga-click="Footer, go to privacy, text:privacy" href="https://github.com/site/privacy">Privacy</a></li>
        <li class="mr-3"><a data-ga-click="Footer, go to security, text:security" href="https://github.com/security">Security</a></li>
        <li class="mr-3"><a href="https://githubstatus.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a data-ga-click="Footer, go to help, text:help" href="https://help.github.com">Help</a></li>
    </ul>

    <a aria-label="Homepage" title="GitHub" class="footer-octicon mr-lg-4" href="https://github.com">
      <svg height="24" class="octicon octicon-mark-github" viewBox="0 0 16 16" version="1.1" width="24" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
</a>
   <ul class="list-style-none d-flex flex-wrap ">
        <li class="mr-3"><a data-ga-click="Footer, go to contact, text:contact" href="https://github.com/contact">Contact GitHub</a></li>
        <li class="mr-3"><a href="https://github.com/pricing" data-ga-click="Footer, go to Pricing, text:Pricing">Pricing</a></li>
      <li class="mr-3"><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li class="mr-3"><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
        <li class="mr-3"><a href="https://github.blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a data-ga-click="Footer, go to about, text:about" href="https://github.com/about">About</a></li>

    </ul>
  </div>
  <div class="d-flex flex-justify-center pb-6">
    <span class="f6 text-gray-light"></span>
  </div>
</div>



  <div id="ajax-error-message" class="ajax-error-message flash flash-error">
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.893 1.5c-.183-.31-.52-.5-.887-.5s-.703.19-.886.5L.138 13.499a.98.98 0 0 0 0 1.001c.193.31.53.501.886.501h13.964c.367 0 .704-.19.877-.5a1.03 1.03 0 0 0 .01-1.002L8.893 1.5zm.133 11.497H6.987v-2.003h2.039v2.003zm0-3.004H6.987V5.987h2.039v4.006z"/></svg>
    <button type="button" class="flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
      <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
    </button>
    You can’t perform that action at this time.
  </div>


    <script crossorigin="anonymous" integrity="sha512-DiQPbGWa0ALOwLs02fk5hmD72O2vgBbk95bHBIgqW0LwS8rjQPrv/NBhNnINkjmpEwQWrnX8hwEG0pfL8ptluw==" type="application/javascript" src="https://github.githubassets.com/assets/compat-bootstrap-4857aac6.js"></script>
    <script crossorigin="anonymous" integrity="sha512-m5ePezkSVci2BjEQk9se9KKv8D0Uwr77F1JC+wrK4+807Jac+06CMzwFmzgltBDcqIzenQOZkg8ZYqzTUOBjZQ==" type="application/javascript" src="https://github.githubassets.com/assets/frameworks-b102e868.js"></script>
    
    <script crossorigin="anonymous" async="async" integrity="sha512-EvJFOCq6/jfp6Hf6HYMUi+3uxaxiE8ohfnE9fQYK2wSDCNDVpKSictscXZwUTK34zNXw4j/L74ncvpydlaI8Bw==" type="application/javascript" src="https://github.githubassets.com/assets/github-bootstrap-0c704aff.js"></script>
    
    
    
  <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner d-none">
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.893 1.5c-.183-.31-.52-.5-.887-.5s-.703.19-.886.5L.138 13.499a.98.98 0 0 0 0 1.001c.193.31.53.501.886.501h13.964c.367 0 .704-.19.877-.5a1.03 1.03 0 0 0 .01-1.002L8.893 1.5zm.133 11.497H6.987v-2.003h2.039v2.003zm0-3.004H6.987V5.987h2.039v4.006z"/></svg>
    <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
    <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
  </div>
  <template id="site-details-dialog">
  <details class="details-reset details-overlay details-overlay-dark lh-default text-gray-dark" open>
    <summary aria-haspopup="dialog" aria-label="Close dialog"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast">
      <button class="Box-btn-octicon m-0 btn-octicon position-absolute right-0 top-0" type="button" aria-label="Close dialog" data-close-dialog>
        <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
      </button>
      <div class="octocat-spinner my-6 js-details-dialog-spinner"></div>
    </details-dialog>
  </details>
</template>

  <div class="Popover js-hovercard-content position-absolute" style="display: none; outline: none;" tabindex="0">
  <div class="Popover-message Popover-message--bottom-left Popover-message--large Box box-shadow-large" style="width:360px;">
  </div>
</div>

  <div aria-live="polite" class="js-global-screen-reader-notice sr-only"></div>

  </body>
</html>

