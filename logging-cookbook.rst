





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
  
  <title>cpython/logging-cookbook.rst at master · python/cpython · GitHub</title>
    <meta name="description" content="The Python programming language. Contribute to python/cpython development by creating an account on GitHub.">
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
  <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
  <meta property="fb:app_id" content="1401488693436528">

    
    <meta property="og:image" content="https://avatars2.githubusercontent.com/u/1525981?s=400&amp;v=4" /><meta property="og:site_name" content="GitHub" /><meta property="og:type" content="object" /><meta property="og:title" content="python/cpython" /><meta property="og:url" content="https://github.com/python/cpython" /><meta property="og:description" content="The Python programming language. Contribute to python/cpython development by creating an account on GitHub." />

  <link rel="assets" href="https://github.githubassets.com/">
  
  <meta name="pjax-timeout" content="1000">
  
  <meta name="request-id" content="96C8:30DD0:15C63A:20AFD1:5C77B5FC" data-pjax-transient>


  

  <meta name="selected-link" value="repo_source" data-pjax-transient>

      <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
    <meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-site-verification" content="GXs5KoUUkNCoaAZn7wPN-t01Pywp9M3sEjnt_3_ZWPc">

  <meta name="octolytics-host" content="collector.githubapp.com" /><meta name="octolytics-app-id" content="github" /><meta name="octolytics-event-url" content="https://collector.githubapp.com/github-external/browser_event" /><meta name="octolytics-dimension-request_id" content="96C8:30DD0:15C63A:20AFD1:5C77B5FC" /><meta name="octolytics-dimension-region_edge" content="ams" /><meta name="octolytics-dimension-region_render" content="iad" />
<meta name="analytics-location" content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" />



    <meta name="google-analytics" content="UA-3769691-2">


<meta class="js-ga-set" name="dimension1" content="Logged Out">



  

      <meta name="hostname" content="github.com">
    <meta name="user-login" content="">

      <meta name="expected-hostname" content="github.com">
    <meta name="js-proxy-site-detection-payload" content="YjJmZWY1NzgzODc2ZTIxYTZkYmQ3ZGQ0NmI1MDE1ZTc3YjZlMDU1NjQzOWExZDEyM2IyNDMzMTIzYjRjZTg1ZXx7InJlbW90ZV9hZGRyZXNzIjoiOTIuOTEuMjIxLjIxOCIsInJlcXVlc3RfaWQiOiI5NkM4OjMwREQwOjE1QzYzQToyMEFGRDE6NUM3N0I1RkMiLCJ0aW1lc3RhbXAiOjE1NTEzNDkyNDQsImhvc3QiOiJnaXRodWIuY29tIn0=">

    <meta name="enabled-features" content="UNIVERSE_BANNER,MARKETPLACE_SOCIAL_PROOF,MARKETPLACE_PLAN_RESTRICTION_EDITOR,MARKETPLACE_BROWSING_V2">

  <meta name="html-safe-nonce" content="b21517502f0f69a6e488156988d447db1c9f7317">

  <meta http-equiv="x-pjax-version" content="51633f82d41fbb109c08bc27389aacb1">
  

      <link href="https://github.com/python/cpython/commits/master.atom" rel="alternate" title="Recent Commits to cpython:master" type="application/atom+xml">

  <meta name="go-import" content="github.com/python/cpython git https://github.com/python/cpython.git">

  <meta name="octolytics-dimension-user_id" content="1525981" /><meta name="octolytics-dimension-user_login" content="python" /><meta name="octolytics-dimension-repository_id" content="81598961" /><meta name="octolytics-dimension-repository_nwo" content="python/cpython" /><meta name="octolytics-dimension-repository_public" content="true" /><meta name="octolytics-dimension-repository_is_fork" content="false" /><meta name="octolytics-dimension-repository_network_root_id" content="81598961" /><meta name="octolytics-dimension-repository_network_root_nwo" content="python/cpython" /><meta name="octolytics-dimension-repository_explore_github_marketplace_ci_cta_shown" content="false" />


    <link rel="canonical" href="https://github.com/python/cpython/blob/master/Doc/howto/logging-cookbook.rst" data-pjax-transient>


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
          data-jump-to-suggestions-path="/_graphql/GetSuggestedNavigationDestinations#csrf-token=Gb0uuWestpkP4iIcWusgKTlBBY+paklX9ODbCRRx2XBK529optTULeNE4/YPX0r0FYwF/CgPbSAB0wz12ka7Xg=="
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

        <a class="HeaderMenu-link no-underline mr-3" href="/login?return_to=%2Fpython%2Fcpython%2Fblob%2Fmaster%2FDoc%2Fhowto%2Flogging-cookbook.rst" data-ga-click="(Logged out) Header, clicked Sign in, text:sign-in">Sign&nbsp;in</a>
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

    
    



  
    <a class="d-none js-permalink-shortcut" data-hotkey="y" href="/python/cpython/blob/4173772031747a9b249be4100b4aa9eda805ea23/Doc/howto/logging-cookbook.rst">Permalink</a>

    <!-- blob contrib key: blob_contributors:v21:5bf7f78ff156e68141a26556c004d4b3 -->

        <div class="signup-prompt-bg rounded-1">
      <div class="signup-prompt p-4 text-center mb-4 rounded-1">
        <div class="position-relative">
          <!-- '"` --><!-- </textarea></xmp> --></option></form><form action="/site/dismiss_signup_prompt" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="4tkG5i6yUIJW34C8FIvNAP5M1z6+L8CkP9OSgG2QvGOc1J0pimGHxN/LfOorKQ+Q+jRnmcYmPdmC5oh97XHHtg==" />
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

  <details-menu class="select-menu-modal position-absolute" style="z-index: 99;" src="/python/cpython/ref-list/master/Doc/howto/logging-cookbook.rst?source_action=show&amp;source_controller=blob" preload>
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
        <span class="repo-root js-repo-root"><span class="js-path-segment"><a data-pjax="true" href="/python/cpython"><span>cpython</span></a></span></span><span class="separator">/</span><span class="js-path-segment"><a data-pjax="true" href="/python/cpython/tree/master/Doc"><span>Doc</span></a></span><span class="separator">/</span><span class="js-path-segment"><a data-pjax="true" href="/python/cpython/tree/master/Doc/howto"><span>howto</span></a></span><span class="separator">/</span><strong class="final-path">logging-cookbook.rst</strong>
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
    
    <span><strong>15</strong> contributors</span>
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
              <a class="link-gray-dark no-underline" href="/birkenfeld">
                <img class="avatar mr-2" alt="" src="https://avatars2.githubusercontent.com/u/144359?s=40&amp;v=4" width="20" height="20" />
                birkenfeld
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/serhiy-storchaka">
                <img class="avatar mr-2" alt="" src="https://avatars0.githubusercontent.com/u/3659035?s=40&amp;v=4" width="20" height="20" />
                serhiy-storchaka
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/ezio-melotti">
                <img class="avatar mr-2" alt="" src="https://avatars3.githubusercontent.com/u/25624924?s=40&amp;v=4" width="20" height="20" />
                ezio-melotti
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/berkerpeksag">
                <img class="avatar mr-2" alt="" src="https://avatars0.githubusercontent.com/u/26338?s=40&amp;v=4" width="20" height="20" />
                berkerpeksag
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/vadmium">
                <img class="avatar mr-2" alt="" src="https://avatars2.githubusercontent.com/u/1024659?s=40&amp;v=4" width="20" height="20" />
                vadmium
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/rhettinger">
                <img class="avatar mr-2" alt="" src="https://avatars3.githubusercontent.com/u/1623689?s=40&amp;v=4" width="20" height="20" />
                rhettinger
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/yuji38kwmt">
                <img class="avatar mr-2" alt="" src="https://avatars0.githubusercontent.com/u/6350027?s=40&amp;v=4" width="20" height="20" />
                yuji38kwmt
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/pablogsal">
                <img class="avatar mr-2" alt="" src="https://avatars3.githubusercontent.com/u/11718525?s=40&amp;v=4" width="20" height="20" />
                pablogsal
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/jamesfe">
                <img class="avatar mr-2" alt="" src="https://avatars1.githubusercontent.com/u/3836461?s=40&amp;v=4" width="20" height="20" />
                jamesfe
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/maggyero">
                <img class="avatar mr-2" alt="" src="https://avatars1.githubusercontent.com/u/33548838?s=40&amp;v=4" width="20" height="20" />
                maggyero
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/delirious-lettuce">
                <img class="avatar mr-2" alt="" src="https://avatars0.githubusercontent.com/u/24502053?s=40&amp;v=4" width="20" height="20" />
                delirious-lettuce
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/csabella">
                <img class="avatar mr-2" alt="" src="https://avatars0.githubusercontent.com/u/25619791?s=40&amp;v=4" width="20" height="20" />
                csabella
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/brettcannon">
                <img class="avatar mr-2" alt="" src="https://avatars1.githubusercontent.com/u/54418?s=40&amp;v=4" width="20" height="20" />
                brettcannon
</a>            </li>
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/asvetlov">
                <img class="avatar mr-2" alt="" src="https://avatars1.githubusercontent.com/u/356399?s=40&amp;v=4" width="20" height="20" />
                asvetlov
</a>            </li>
        </ul>

  </details-dialog>
</details>
          <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=130553" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=vsajip">
      <img class="avatar" src="https://avatars1.githubusercontent.com/u/130553?s=40&amp;v=4" width="20" height="20" alt="@vsajip" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=144359" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=birkenfeld">
      <img class="avatar" src="https://avatars2.githubusercontent.com/u/144359?s=40&amp;v=4" width="20" height="20" alt="@birkenfeld" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=3659035" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=serhiy-storchaka">
      <img class="avatar" src="https://avatars0.githubusercontent.com/u/3659035?s=40&amp;v=4" width="20" height="20" alt="@serhiy-storchaka" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=25624924" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=ezio-melotti">
      <img class="avatar" src="https://avatars3.githubusercontent.com/u/25624924?s=40&amp;v=4" width="20" height="20" alt="@ezio-melotti" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=26338" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=berkerpeksag">
      <img class="avatar" src="https://avatars0.githubusercontent.com/u/26338?s=40&amp;v=4" width="20" height="20" alt="@berkerpeksag" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=1024659" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=vadmium">
      <img class="avatar" src="https://avatars2.githubusercontent.com/u/1024659?s=40&amp;v=4" width="20" height="20" alt="@vadmium" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=1623689" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=rhettinger">
      <img class="avatar" src="https://avatars3.githubusercontent.com/u/1623689?s=40&amp;v=4" width="20" height="20" alt="@rhettinger" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=6350027" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=yuji38kwmt">
      <img class="avatar" src="https://avatars0.githubusercontent.com/u/6350027?s=40&amp;v=4" width="20" height="20" alt="@yuji38kwmt" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=11718525" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=pablogsal">
      <img class="avatar" src="https://avatars3.githubusercontent.com/u/11718525?s=40&amp;v=4" width="20" height="20" alt="@pablogsal" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=3836461" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=jamesfe">
      <img class="avatar" src="https://avatars1.githubusercontent.com/u/3836461?s=40&amp;v=4" width="20" height="20" alt="@jamesfe" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=33548838" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=maggyero">
      <img class="avatar" src="https://avatars1.githubusercontent.com/u/33548838?s=40&amp;v=4" width="20" height="20" alt="@maggyero" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=24502053" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=delirious-lettuce">
      <img class="avatar" src="https://avatars0.githubusercontent.com/u/24502053?s=40&amp;v=4" width="20" height="20" alt="@delirious-lettuce" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=25619791" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=csabella">
      <img class="avatar" src="https://avatars0.githubusercontent.com/u/25619791?s=40&amp;v=4" width="20" height="20" alt="@csabella" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=54418" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=brettcannon">
      <img class="avatar" src="https://avatars1.githubusercontent.com/u/54418?s=40&amp;v=4" width="20" height="20" alt="@brettcannon" /> 
</a>    <a class="avatar-link" data-hovercard-type="user" data-hovercard-url="/hovercards?user_id=356399" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst?author=asvetlov">
      <img class="avatar" src="https://avatars1.githubusercontent.com/u/356399?s=40&amp;v=4" width="20" height="20" alt="@asvetlov" /> 
</a>

    </div>
  </div>





    <div class="file ">
      
<div class="file-header ">
  
  <div class="file-info float-left ">
      2712 lines (2206 sloc)
      <span class="file-info-divider"></span>
    105 KB
  </div>

  <div class="file-actions d-flex ">

    <div class="BtnGroup">
      <a id="raw-url" class="btn btn-sm BtnGroup-item" href="/python/cpython/raw/master/Doc/howto/logging-cookbook.rst">Raw</a>
        <a class="btn btn-sm js-update-url-with-hash BtnGroup-item" data-hotkey="b" href="/python/cpython/blame/master/Doc/howto/logging-cookbook.rst">Blame</a>
      <a rel="nofollow" class="btn btn-sm BtnGroup-item" href="/python/cpython/commits/master/Doc/howto/logging-cookbook.rst">History</a>
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
    <article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-logging-cookbook" class="anchor" aria-hidden="true" href="#logging-cookbook"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Logging Cookbook</h1>
<table frame="void" rules="none">


<tbody valign="top">
<tr><th>Author:</th>
<td>Vinay Sajip &lt;vinay_sajip at red-dove dot com&gt;</td></tr>
</tbody>
</table>
<p>This page contains a number of recipes related to logging, which have been found
useful in the past.</p>
<pre>.. currentmodule:: logging

</pre>
<a name="user-content-using-logging-in-multiple-modules"></a>
<h2><a id="user-content-using-logging-in-multiple-modules" class="anchor" aria-hidden="true" href="#using-logging-in-multiple-modules"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Using logging in multiple modules</h2>
<p>Multiple calls to <code>logging.getLogger('someLogger')</code> return a reference to the
same logger object.  This is true not only within the same module, but also
across modules as long as it is in the same Python interpreter process.  It is
true for references to the same object; additionally, application code can
define and configure a parent logger in one module and create (but not
configure) a child logger in a separate module, and all logger calls to the
child will pass up to the parent.  Here is a main module:</p>
<pre>import logging
import auxiliary_module

# create logger with 'spam_application'
logger = logging.getLogger('spam_application')
logger.setLevel(logging.DEBUG)
# create file handler which logs even debug messages
fh = logging.FileHandler('spam.log')
fh.setLevel(logging.DEBUG)
# create console handler with a higher log level
ch = logging.StreamHandler()
ch.setLevel(logging.ERROR)
# create formatter and add it to the handlers
formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
fh.setFormatter(formatter)
ch.setFormatter(formatter)
# add the handlers to the logger
logger.addHandler(fh)
logger.addHandler(ch)

logger.info('creating an instance of auxiliary_module.Auxiliary')
a = auxiliary_module.Auxiliary()
logger.info('created an instance of auxiliary_module.Auxiliary')
logger.info('calling auxiliary_module.Auxiliary.do_something')
a.do_something()
logger.info('finished auxiliary_module.Auxiliary.do_something')
logger.info('calling auxiliary_module.some_function()')
auxiliary_module.some_function()
logger.info('done with auxiliary_module.some_function()')
</pre>
<p>Here is the auxiliary module:</p>
<pre>import logging

# create logger
module_logger = logging.getLogger('spam_application.auxiliary')

class Auxiliary:
    def __init__(self):
        self.logger = logging.getLogger('spam_application.auxiliary.Auxiliary')
        self.logger.info('creating an instance of Auxiliary')

    def do_something(self):
        self.logger.info('doing something')
        a = 1 + 1
        self.logger.info('done doing something')

def some_function():
    module_logger.info('received a call to "some_function"')
</pre>
<p>The output looks like this:</p>
<pre lang="none">2005-03-23 23:47:11,663 - spam_application - INFO -
   creating an instance of auxiliary_module.Auxiliary
2005-03-23 23:47:11,665 - spam_application.auxiliary.Auxiliary - INFO -
   creating an instance of Auxiliary
2005-03-23 23:47:11,665 - spam_application - INFO -
   created an instance of auxiliary_module.Auxiliary
2005-03-23 23:47:11,668 - spam_application - INFO -
   calling auxiliary_module.Auxiliary.do_something
2005-03-23 23:47:11,668 - spam_application.auxiliary.Auxiliary - INFO -
   doing something
2005-03-23 23:47:11,669 - spam_application.auxiliary.Auxiliary - INFO -
   done doing something
2005-03-23 23:47:11,670 - spam_application - INFO -
   finished auxiliary_module.Auxiliary.do_something
2005-03-23 23:47:11,671 - spam_application - INFO -
   calling auxiliary_module.some_function()
2005-03-23 23:47:11,672 - spam_application.auxiliary - INFO -
   received a call to 'some_function'
2005-03-23 23:47:11,673 - spam_application - INFO -
   done with auxiliary_module.some_function()
</pre>
<a name="user-content-logging-from-multiple-threads"></a>
<h2><a id="user-content-logging-from-multiple-threads" class="anchor" aria-hidden="true" href="#logging-from-multiple-threads"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Logging from multiple threads</h2>
<p>Logging from multiple threads requires no special effort. The following example
shows logging from the main (initial) thread and another thread:</p>
<pre>import logging
import threading
import time

def worker(arg):
    while not arg['stop']:
        logging.debug('Hi from myfunc')
        time.sleep(0.5)

def main():
    logging.basicConfig(level=logging.DEBUG, format='%(relativeCreated)6d %(threadName)s %(message)s')
    info = {'stop': False}
    thread = threading.Thread(target=worker, args=(info,))
    thread.start()
    while True:
        try:
            logging.debug('Hello from main')
            time.sleep(0.75)
        except KeyboardInterrupt:
            info['stop'] = True
            break
    thread.join()

if __name__ == '__main__':
    main()
</pre>
<p>When run, the script should print something like the following:</p>
<pre lang="none">   0 Thread-1 Hi from myfunc
   3 MainThread Hello from main
 505 Thread-1 Hi from myfunc
 755 MainThread Hello from main
1007 Thread-1 Hi from myfunc
1507 MainThread Hello from main
1508 Thread-1 Hi from myfunc
2010 Thread-1 Hi from myfunc
2258 MainThread Hello from main
2512 Thread-1 Hi from myfunc
3009 MainThread Hello from main
3013 Thread-1 Hi from myfunc
3515 Thread-1 Hi from myfunc
3761 MainThread Hello from main
4017 Thread-1 Hi from myfunc
4513 MainThread Hello from main
4518 Thread-1 Hi from myfunc
</pre>
<p>This shows the logging output interspersed as one might expect. This approach
works for more threads than shown here, of course.</p>
<a name="user-content-multiple-handlers-and-formatters"></a>
<h2><a id="user-content-multiple-handlers-and-formatters" class="anchor" aria-hidden="true" href="#multiple-handlers-and-formatters"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Multiple handlers and formatters</h2>
<p>Loggers are plain Python objects.  The <a href="#id2"><span id="user-content-id3">:meth:`~Logger.addHandler`</span></a> method has no
minimum or maximum quota for the number of handlers you may add.  Sometimes it
will be beneficial for an application to log all messages of all severities to a
text file while simultaneously logging errors or above to the console.  To set
this up, simply configure the appropriate handlers.  The logging calls in the
application code will remain unchanged.  Here is a slight modification to the
previous simple module-based configuration example:</p>
<pre>import logging

logger = logging.getLogger('simple_example')
logger.setLevel(logging.DEBUG)
# create file handler which logs even debug messages
fh = logging.FileHandler('spam.log')
fh.setLevel(logging.DEBUG)
# create console handler with a higher log level
ch = logging.StreamHandler()
ch.setLevel(logging.ERROR)
# create formatter and add it to the handlers
formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
ch.setFormatter(formatter)
fh.setFormatter(formatter)
# add the handlers to logger
logger.addHandler(ch)
logger.addHandler(fh)

# 'application' code
logger.debug('debug message')
logger.info('info message')
logger.warning('warn message')
logger.error('error message')
logger.critical('critical message')
</pre>
<p>Notice that the 'application' code does not care about multiple handlers.  All
that changed was the addition and configuration of a new handler named <em>fh</em>.</p>
<p>The ability to create new handlers with higher- or lower-severity filters can be
very helpful when writing and testing an application.  Instead of using many
<code>print</code> statements for debugging, use <code>logger.debug</code>: Unlike the print
statements, which you will have to delete or comment out later, the logger.debug
statements can remain intact in the source code and remain dormant until you
need them again.  At that time, the only change that needs to happen is to
modify the severity level of the logger and/or handler to debug.</p>
<a name="user-content-logging-to-multiple-destinations"></a>
<h2><a id="user-content-logging-to-multiple-destinations" class="anchor" aria-hidden="true" href="#logging-to-multiple-destinations"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Logging to multiple destinations</h2>
<p>Let's say you want to log to console and file with different message formats and
in differing circumstances. Say you want to log messages with levels of DEBUG
and higher to file, and those messages at level INFO and higher to the console.
Let's also assume that the file should contain timestamps, but the console
messages should not. Here's how you can achieve this:</p>
<pre>import logging

# set up logging to file - see previous section for more details
logging.basicConfig(level=logging.DEBUG,
                    format='%(asctime)s %(name)-12s %(levelname)-8s %(message)s',
                    datefmt='%m-%d %H:%M',
                    filename='/temp/myapp.log',
                    filemode='w')
# define a Handler which writes INFO messages or higher to the sys.stderr
console = logging.StreamHandler()
console.setLevel(logging.INFO)
# set a format which is simpler for console use
formatter = logging.Formatter('%(name)-12s: %(levelname)-8s %(message)s')
# tell the handler to use this format
console.setFormatter(formatter)
# add the handler to the root logger
logging.getLogger('').addHandler(console)

# Now, we can log to the root logger, or any other logger. First the root...
logging.info('Jackdaws love my big sphinx of quartz.')

# Now, define a couple of other loggers which might represent areas in your
# application:

logger1 = logging.getLogger('myapp.area1')
logger2 = logging.getLogger('myapp.area2')

logger1.debug('Quick zephyrs blow, vexing daft Jim.')
logger1.info('How quickly daft jumping zebras vex.')
logger2.warning('Jail zesty vixen who grabbed pay from quack.')
logger2.error('The five boxing wizards jump quickly.')
</pre>
<p>When you run this, on the console you will see</p>
<pre lang="none">root        : INFO     Jackdaws love my big sphinx of quartz.
myapp.area1 : INFO     How quickly daft jumping zebras vex.
myapp.area2 : WARNING  Jail zesty vixen who grabbed pay from quack.
myapp.area2 : ERROR    The five boxing wizards jump quickly.
</pre>
<p>and in the file you will see something like</p>
<pre lang="none">10-22 22:19 root         INFO     Jackdaws love my big sphinx of quartz.
10-22 22:19 myapp.area1  DEBUG    Quick zephyrs blow, vexing daft Jim.
10-22 22:19 myapp.area1  INFO     How quickly daft jumping zebras vex.
10-22 22:19 myapp.area2  WARNING  Jail zesty vixen who grabbed pay from quack.
10-22 22:19 myapp.area2  ERROR    The five boxing wizards jump quickly.
</pre>
<p>As you can see, the DEBUG message only shows up in the file. The other messages
are sent to both destinations.</p>
<p>This example uses console and file handlers, but you can use any number and
combination of handlers you choose.</p>
<a name="user-content-configuration-server-example"></a>
<h2><a id="user-content-configuration-server-example" class="anchor" aria-hidden="true" href="#configuration-server-example"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Configuration server example</h2>
<p>Here is an example of a module using the logging configuration server:</p>
<pre>import logging
import logging.config
import time
import os

# read initial config file
logging.config.fileConfig('logging.conf')

# create and start listener on port 9999
t = logging.config.listen(9999)
t.start()

logger = logging.getLogger('simpleExample')

try:
    # loop through logging calls to see the difference
    # new configurations make, until Ctrl+C is pressed
    while True:
        logger.debug('debug message')
        logger.info('info message')
        logger.warning('warn message')
        logger.error('error message')
        logger.critical('critical message')
        time.sleep(5)
except KeyboardInterrupt:
    # cleanup
    logging.config.stopListening()
    t.join()
</pre>
<p>And here is a script that takes a filename and sends that file to the server,
properly preceded with the binary-encoded length, as the new logging
configuration:</p>
<pre>#!/usr/bin/env python
import socket, sys, struct

with open(sys.argv[1], 'rb') as f:
    data_to_send = f.read()

HOST = 'localhost'
PORT = 9999
s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
print('connecting...')
s.connect((HOST, PORT))
print('sending config...')
s.send(struct.pack('&gt;L', len(data_to_send)))
s.send(data_to_send)
s.close()
print('complete')
</pre>
<a name="user-content-dealing-with-handlers-that-block"></a>
<h2><a id="user-content-dealing-with-handlers-that-block" class="anchor" aria-hidden="true" href="#dealing-with-handlers-that-block"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Dealing with handlers that block</h2>
<pre>.. currentmodule:: logging.handlers

</pre>
<p>Sometimes you have to get your logging handlers to do their work without
blocking the thread you're logging from. This is common in Web applications,
though of course it also occurs in other scenarios.</p>
<p>A common culprit which demonstrates sluggish behaviour is the
<a href="#id4"><span id="user-content-id5">:class:`SMTPHandler`</span></a>: sending emails can take a long time, for a
number of reasons outside the developer's control (for example, a poorly
performing mail or network infrastructure). But almost any network-based
handler can block: Even a <a href="#id6"><span id="user-content-id7">:class:`SocketHandler`</span></a> operation may do a
DNS query under the hood which is too slow (and this query can be deep in the
socket library code, below the Python layer, and outside your control).</p>
<p>One solution is to use a two-part approach. For the first part, attach only a
<a href="#id8"><span id="user-content-id9">:class:`QueueHandler`</span></a> to those loggers which are accessed from
performance-critical threads. They simply write to their queue, which can be
sized to a large enough capacity or initialized with no upper bound to their
size. The write to the queue will typically be accepted quickly, though you
will probably need to catch the <a href="#id10"><span id="user-content-id11">:exc:`queue.Full`</span></a> exception as a precaution
in your code. If you are a library developer who has performance-critical
threads in their code, be sure to document this (together with a suggestion to
attach only <code>QueueHandlers</code> to your loggers) for the benefit of other
developers who will use your code.</p>
<p>The second part of the solution is <a href="#id12"><span id="user-content-id13">:class:`QueueListener`</span></a>, which has been
designed as the counterpart to <a href="#id14"><span id="user-content-id15">:class:`QueueHandler`</span></a>.  A
<a href="#id16"><span id="user-content-id17">:class:`QueueListener`</span></a> is very simple: it's passed a queue and some handlers,
and it fires up an internal thread which listens to its queue for LogRecords
sent from <code>QueueHandlers</code> (or any other source of <code>LogRecords</code>, for that
matter). The <code>LogRecords</code> are removed from the queue and passed to the
handlers for processing.</p>
<p>The advantage of having a separate <a href="#id18"><span id="user-content-id19">:class:`QueueListener`</span></a> class is that you
can use the same instance to service multiple <code>QueueHandlers</code>. This is more
resource-friendly than, say, having threaded versions of the existing handler
classes, which would eat up one thread per handler for no particular benefit.</p>
<p>An example of using these two classes follows (imports omitted):</p>
<pre>que = queue.Queue(-1)  # no limit on size
queue_handler = QueueHandler(que)
handler = logging.StreamHandler()
listener = QueueListener(que, handler)
root = logging.getLogger()
root.addHandler(queue_handler)
formatter = logging.Formatter('%(threadName)s: %(message)s')
handler.setFormatter(formatter)
listener.start()
# The log output will display the thread which generated
# the event (the main thread) rather than the internal
# thread which monitors the internal queue. This is what
# you want to happen.
root.warning('Look out!')
listener.stop()
</pre>
<p>which, when run, will produce:</p>
<pre lang="none">MainThread: Look out!
</pre>
<pre>.. versionchanged:: 3.5
   Prior to Python 3.5, the :class:`QueueListener` always passed every message
   received from the queue to every handler it was initialized with. (This was
   because it was assumed that level filtering was all done on the other side,
   where the queue is filled.) From 3.5 onwards, this behaviour can be changed
   by passing a keyword argument ``respect_handler_level=True`` to the
   listener's constructor. When this is done, the listener compares the level
   of each message with the handler's level, and only passes a message to a
   handler if it's appropriate to do so.

</pre>
<a name="user-content-sending-and-receiving-logging-events-across-a-network"></a>
<h2><a id="user-content-sending-and-receiving-logging-events-across-a-network" class="anchor" aria-hidden="true" href="#sending-and-receiving-logging-events-across-a-network"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Sending and receiving logging events across a network</h2>
<p>Let's say you want to send logging events across a network, and handle them at
the receiving end. A simple way of doing this is attaching a
<a href="#id20"><span id="user-content-id21">:class:`SocketHandler`</span></a> instance to the root logger at the sending end:</p>
<pre>import logging, logging.handlers

rootLogger = logging.getLogger('')
rootLogger.setLevel(logging.DEBUG)
socketHandler = logging.handlers.SocketHandler('localhost',
                    logging.handlers.DEFAULT_TCP_LOGGING_PORT)
# don't bother with a formatter, since a socket handler sends the event as
# an unformatted pickle
rootLogger.addHandler(socketHandler)

# Now, we can log to the root logger, or any other logger. First the root...
logging.info('Jackdaws love my big sphinx of quartz.')

# Now, define a couple of other loggers which might represent areas in your
# application:

logger1 = logging.getLogger('myapp.area1')
logger2 = logging.getLogger('myapp.area2')

logger1.debug('Quick zephyrs blow, vexing daft Jim.')
logger1.info('How quickly daft jumping zebras vex.')
logger2.warning('Jail zesty vixen who grabbed pay from quack.')
logger2.error('The five boxing wizards jump quickly.')
</pre>
<p>At the receiving end, you can set up a receiver using the <a href="#id22"><span id="user-content-id23">:mod:`socketserver`</span></a>
module. Here is a basic working example:</p>
<pre>import pickle
import logging
import logging.handlers
import socketserver
import struct


class LogRecordStreamHandler(socketserver.StreamRequestHandler):
    """Handler for a streaming logging request.

    This basically logs the record using whatever logging policy is
    configured locally.
    """

    def handle(self):
        """
        Handle multiple requests - each expected to be a 4-byte length,
        followed by the LogRecord in pickle format. Logs the record
        according to whatever policy is configured locally.
        """
        while True:
            chunk = self.connection.recv(4)
            if len(chunk) &lt; 4:
                break
            slen = struct.unpack('&gt;L', chunk)[0]
            chunk = self.connection.recv(slen)
            while len(chunk) &lt; slen:
                chunk = chunk + self.connection.recv(slen - len(chunk))
            obj = self.unPickle(chunk)
            record = logging.makeLogRecord(obj)
            self.handleLogRecord(record)

    def unPickle(self, data):
        return pickle.loads(data)

    def handleLogRecord(self, record):
        # if a name is specified, we use the named logger rather than the one
        # implied by the record.
        if self.server.logname is not None:
            name = self.server.logname
        else:
            name = record.name
        logger = logging.getLogger(name)
        # N.B. EVERY record gets logged. This is because Logger.handle
        # is normally called AFTER logger-level filtering. If you want
        # to do filtering, do it at the client end to save wasting
        # cycles and network bandwidth!
        logger.handle(record)

class LogRecordSocketReceiver(socketserver.ThreadingTCPServer):
    """
    Simple TCP socket-based logging receiver suitable for testing.
    """

    allow_reuse_address = True

    def __init__(self, host='localhost',
                 port=logging.handlers.DEFAULT_TCP_LOGGING_PORT,
                 handler=LogRecordStreamHandler):
        socketserver.ThreadingTCPServer.__init__(self, (host, port), handler)
        self.abort = 0
        self.timeout = 1
        self.logname = None

    def serve_until_stopped(self):
        import select
        abort = 0
        while not abort:
            rd, wr, ex = select.select([self.socket.fileno()],
                                       [], [],
                                       self.timeout)
            if rd:
                self.handle_request()
            abort = self.abort

def main():
    logging.basicConfig(
        format='%(relativeCreated)5d %(name)-15s %(levelname)-8s %(message)s')
    tcpserver = LogRecordSocketReceiver()
    print('About to start TCP server...')
    tcpserver.serve_until_stopped()

if __name__ == '__main__':
    main()
</pre>
<p>First run the server, and then the client. On the client side, nothing is
printed on the console; on the server side, you should see something like:</p>
<pre lang="none">About to start TCP server...
   59 root            INFO     Jackdaws love my big sphinx of quartz.
   59 myapp.area1     DEBUG    Quick zephyrs blow, vexing daft Jim.
   69 myapp.area1     INFO     How quickly daft jumping zebras vex.
   69 myapp.area2     WARNING  Jail zesty vixen who grabbed pay from quack.
   69 myapp.area2     ERROR    The five boxing wizards jump quickly.
</pre>
<p>Note that there are some security issues with pickle in some scenarios. If
these affect you, you can use an alternative serialization scheme by overriding
the <a href="#id24"><span id="user-content-id25">:meth:`~handlers.SocketHandler.makePickle`</span></a> method and implementing your
alternative there, as well as adapting the above script to use your alternative
serialization.</p>
<a name="user-content-adding-contextual-information-to-your-logging-output"></a>
<h2><a id="user-content-adding-contextual-information-to-your-logging-output" class="anchor" aria-hidden="true" href="#adding-contextual-information-to-your-logging-output"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Adding contextual information to your logging output</h2>
<p>Sometimes you want logging output to contain contextual information in
addition to the parameters passed to the logging call. For example, in a
networked application, it may be desirable to log client-specific information
in the log (e.g. remote client's username, or IP address). Although you could
use the <em>extra</em> parameter to achieve this, it's not always convenient to pass
the information in this way. While it might be tempting to create
<a href="#id26"><span id="user-content-id27">:class:`Logger`</span></a> instances on a per-connection basis, this is not a good idea
because these instances are not garbage collected. While this is not a problem
in practice, when the number of <a href="#id28"><span id="user-content-id29">:class:`Logger`</span></a> instances is dependent on the
level of granularity you want to use in logging an application, it could
be hard to manage if the number of <a href="#id30"><span id="user-content-id31">:class:`Logger`</span></a> instances becomes
effectively unbounded.</p>
<a name="user-content-using-loggeradapters-to-impart-contextual-information"></a>
<h3><a id="user-content-using-loggeradapters-to-impart-contextual-information" class="anchor" aria-hidden="true" href="#using-loggeradapters-to-impart-contextual-information"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Using LoggerAdapters to impart contextual information</h3>
<p>An easy way in which you can pass contextual information to be output along
with logging event information is to use the <a href="#id32"><span id="user-content-id33">:class:`LoggerAdapter`</span></a> class.
This class is designed to look like a <a href="#id34"><span id="user-content-id35">:class:`Logger`</span></a>, so that you can call
<a href="#id36"><span id="user-content-id37">:meth:`debug`</span></a>, <a href="#id38"><span id="user-content-id39">:meth:`info`</span></a>, <a href="#id40"><span id="user-content-id41">:meth:`warning`</span></a>, <a href="#id42"><span id="user-content-id43">:meth:`error`</span></a>,
<a href="#id44"><span id="user-content-id45">:meth:`exception`</span></a>, <a href="#id46"><span id="user-content-id47">:meth:`critical`</span></a> and <a href="#id48"><span id="user-content-id49">:meth:`log`</span></a>. These methods have the
same signatures as their counterparts in <a href="#id50"><span id="user-content-id51">:class:`Logger`</span></a>, so you can use the
two types of instances interchangeably.</p>
<p>When you create an instance of <a href="#id52"><span id="user-content-id53">:class:`LoggerAdapter`</span></a>, you pass it a
<a href="#id54"><span id="user-content-id55">:class:`Logger`</span></a> instance and a dict-like object which contains your contextual
information. When you call one of the logging methods on an instance of
<a href="#id56"><span id="user-content-id57">:class:`LoggerAdapter`</span></a>, it delegates the call to the underlying instance of
<a href="#id58"><span id="user-content-id59">:class:`Logger`</span></a> passed to its constructor, and arranges to pass the contextual
information in the delegated call. Here's a snippet from the code of
<a href="#id60"><span id="user-content-id61">:class:`LoggerAdapter`</span></a>:</p>
<pre>def debug(self, msg, *args, **kwargs):
    """
    Delegate a debug call to the underlying logger, after adding
    contextual information from this adapter instance.
    """
    msg, kwargs = self.process(msg, kwargs)
    self.logger.debug(msg, *args, **kwargs)
</pre>
<p>The <a href="#id62"><span id="user-content-id63">:meth:`~LoggerAdapter.process`</span></a> method of <a href="#id64"><span id="user-content-id65">:class:`LoggerAdapter`</span></a> is where the
contextual information is added to the logging output. It's passed the message
and keyword arguments of the logging call, and it passes back (potentially)
modified versions of these to use in the call to the underlying logger. The
default implementation of this method leaves the message alone, but inserts
an 'extra' key in the keyword argument whose value is the dict-like object
passed to the constructor. Of course, if you had passed an 'extra' keyword
argument in the call to the adapter, it will be silently overwritten.</p>
<p>The advantage of using 'extra' is that the values in the dict-like object are
merged into the <a href="#id66"><span id="user-content-id67">:class:`LogRecord`</span></a> instance's __dict__, allowing you to use
customized strings with your <a href="#id68"><span id="user-content-id69">:class:`Formatter`</span></a> instances which know about
the keys of the dict-like object. If you need a different method, e.g. if you
want to prepend or append the contextual information to the message string,
you just need to subclass <a href="#id70"><span id="user-content-id71">:class:`LoggerAdapter`</span></a> and override
<a href="#id72"><span id="user-content-id73">:meth:`~LoggerAdapter.process`</span></a> to do what you need. Here is a simple example:</p>
<pre>class CustomAdapter(logging.LoggerAdapter):
    """
    This example adapter expects the passed in dict-like object to have a
    'connid' key, whose value in brackets is prepended to the log message.
    """
    def process(self, msg, kwargs):
        return '[%s] %s' % (self.extra['connid'], msg), kwargs
</pre>
<p>which you can use like this:</p>
<pre>logger = logging.getLogger(__name__)
adapter = CustomAdapter(logger, {'connid': some_conn_id})
</pre>
<p>Then any events that you log to the adapter will have the value of
<code>some_conn_id</code> prepended to the log messages.</p>
<a name="user-content-using-objects-other-than-dicts-to-pass-contextual-information"></a>
<h4><a id="user-content-using-objects-other-than-dicts-to-pass-contextual-information" class="anchor" aria-hidden="true" href="#using-objects-other-than-dicts-to-pass-contextual-information"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Using objects other than dicts to pass contextual information</h4>
<p>You don't need to pass an actual dict to a <a href="#id74"><span id="user-content-id75">:class:`LoggerAdapter`</span></a> - you could
pass an instance of a class which implements <code>__getitem__</code> and <code>__iter__</code> so
that it looks like a dict to logging. This would be useful if you want to
generate values dynamically (whereas the values in a dict would be constant).</p>
<a name="user-content-using-filters-to-impart-contextual-information"></a>
<h3><a id="user-content-using-filters-to-impart-contextual-information" class="anchor" aria-hidden="true" href="#using-filters-to-impart-contextual-information"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Using Filters to impart contextual information</h3>
<p>You can also add contextual information to log output using a user-defined
<a href="#id76"><span id="user-content-id77">:class:`Filter`</span></a>. <code>Filter</code> instances are allowed to modify the <code>LogRecords</code>
passed to them, including adding additional attributes which can then be output
using a suitable format string, or if needed a custom <a href="#id78"><span id="user-content-id79">:class:`Formatter`</span></a>.</p>
<p>For example in a web application, the request being processed (or at least,
the interesting parts of it) can be stored in a threadlocal
(<a href="#id80"><span id="user-content-id81">:class:`threading.local`</span></a>) variable, and then accessed from a <code>Filter</code> to
add, say, information from the request - say, the remote IP address and remote
user's username - to the <code>LogRecord</code>, using the attribute names 'ip' and
'user' as in the <code>LoggerAdapter</code> example above. In that case, the same format
string can be used to get similar output to that shown above. Here's an example
script:</p>
<pre>import logging
from random import choice

class ContextFilter(logging.Filter):
    """
    This is a filter which injects contextual information into the log.

    Rather than use actual contextual information, we just use random
    data in this demo.
    """

    USERS = ['jim', 'fred', 'sheila']
    IPS = ['123.231.231.123', '127.0.0.1', '192.168.0.1']

    def filter(self, record):

        record.ip = choice(ContextFilter.IPS)
        record.user = choice(ContextFilter.USERS)
        return True

if __name__ == '__main__':
    levels = (logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR, logging.CRITICAL)
    logging.basicConfig(level=logging.DEBUG,
                        format='%(asctime)-15s %(name)-5s %(levelname)-8s IP: %(ip)-15s User: %(user)-8s %(message)s')
    a1 = logging.getLogger('a.b.c')
    a2 = logging.getLogger('d.e.f')

    f = ContextFilter()
    a1.addFilter(f)
    a2.addFilter(f)
    a1.debug('A debug message')
    a1.info('An info message with %s', 'some parameters')
    for x in range(10):
        lvl = choice(levels)
        lvlname = logging.getLevelName(lvl)
        a2.log(lvl, 'A message at %s level with %d %s', lvlname, 2, 'parameters')
</pre>
<p>which, when run, produces something like:</p>
<pre lang="none">2010-09-06 22:38:15,292 a.b.c DEBUG    IP: 123.231.231.123 User: fred     A debug message
2010-09-06 22:38:15,300 a.b.c INFO     IP: 192.168.0.1     User: sheila   An info message with some parameters
2010-09-06 22:38:15,300 d.e.f CRITICAL IP: 127.0.0.1       User: sheila   A message at CRITICAL level with 2 parameters
2010-09-06 22:38:15,300 d.e.f ERROR    IP: 127.0.0.1       User: jim      A message at ERROR level with 2 parameters
2010-09-06 22:38:15,300 d.e.f DEBUG    IP: 127.0.0.1       User: sheila   A message at DEBUG level with 2 parameters
2010-09-06 22:38:15,300 d.e.f ERROR    IP: 123.231.231.123 User: fred     A message at ERROR level with 2 parameters
2010-09-06 22:38:15,300 d.e.f CRITICAL IP: 192.168.0.1     User: jim      A message at CRITICAL level with 2 parameters
2010-09-06 22:38:15,300 d.e.f CRITICAL IP: 127.0.0.1       User: sheila   A message at CRITICAL level with 2 parameters
2010-09-06 22:38:15,300 d.e.f DEBUG    IP: 192.168.0.1     User: jim      A message at DEBUG level with 2 parameters
2010-09-06 22:38:15,301 d.e.f ERROR    IP: 127.0.0.1       User: sheila   A message at ERROR level with 2 parameters
2010-09-06 22:38:15,301 d.e.f DEBUG    IP: 123.231.231.123 User: fred     A message at DEBUG level with 2 parameters
2010-09-06 22:38:15,301 d.e.f INFO     IP: 123.231.231.123 User: fred     A message at INFO level with 2 parameters
</pre>
<a name="user-content-logging-to-a-single-file-from-multiple-processes"></a>
<h2><a id="user-content-logging-to-a-single-file-from-multiple-processes" class="anchor" aria-hidden="true" href="#logging-to-a-single-file-from-multiple-processes"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Logging to a single file from multiple processes</h2>
<p>Although logging is thread-safe, and logging to a single file from multiple
threads in a single process <em>is</em> supported, logging to a single file from
<em>multiple processes</em> is <em>not</em> supported, because there is no standard way to
serialize access to a single file across multiple processes in Python. If you
need to log to a single file from multiple processes, one way of doing this is
to have all the processes log to a <a href="#id82"><span id="user-content-id83">:class:`~handlers.SocketHandler`</span></a>, and have a
separate process which implements a socket server which reads from the socket
and logs to file. (If you prefer, you can dedicate one thread in one of the
existing processes to perform this function.)
<a href="#id84"><span id="user-content-id85">:ref:`This section &lt;network-logging&gt;`</span></a> documents this approach in more detail and
includes a working socket receiver which can be used as a starting point for you
to adapt in your own applications.</p>
<p>You could also write your own handler which uses the <a href="#id86"><span id="user-content-id87">:class:`~multiprocessing.Lock`</span></a>
class from the <a href="#id88"><span id="user-content-id89">:mod:`multiprocessing`</span></a> module to serialize access to the
file from your processes. The existing <a href="#id90"><span id="user-content-id91">:class:`FileHandler`</span></a> and subclasses do
not make use of <a href="#id92"><span id="user-content-id93">:mod:`multiprocessing`</span></a> at present, though they may do so in the
future. Note that at present, the <a href="#id94"><span id="user-content-id95">:mod:`multiprocessing`</span></a> module does not provide
working lock functionality on all platforms (see
<a href="https://bugs.python.org/issue3770" rel="nofollow">https://bugs.python.org/issue3770</a>).</p>
<pre>.. currentmodule:: logging.handlers

</pre>
<p>Alternatively, you can use a <code>Queue</code> and a <a href="#id96"><span id="user-content-id97">:class:`QueueHandler`</span></a> to send
all logging events to one of the processes in your multi-process application.
The following example script demonstrates how you can do this; in the example
a separate listener process listens for events sent by other processes and logs
them according to its own logging configuration. Although the example only
demonstrates one way of doing it (for example, you may want to use a listener
thread rather than a separate listener process -- the implementation would be
analogous) it does allow for completely different logging configurations for
the listener and the other processes in your application, and can be used as
the basis for code meeting your own specific requirements:</p>
<pre># You'll need these imports in your own code
import logging
import logging.handlers
import multiprocessing

# Next two import lines for this demo only
from random import choice, random
import time

#
# Because you'll want to define the logging configurations for listener and workers, the
# listener and worker process functions take a configurer parameter which is a callable
# for configuring logging for that process. These functions are also passed the queue,
# which they use for communication.
#
# In practice, you can configure the listener however you want, but note that in this
# simple example, the listener does not apply level or filter logic to received records.
# In practice, you would probably want to do this logic in the worker processes, to avoid
# sending events which would be filtered out between processes.
#
# The size of the rotated files is made small so you can see the results easily.
def listener_configurer():
    root = logging.getLogger()
    h = logging.handlers.RotatingFileHandler('mptest.log', 'a', 300, 10)
    f = logging.Formatter('%(asctime)s %(processName)-10s %(name)s %(levelname)-8s %(message)s')
    h.setFormatter(f)
    root.addHandler(h)

# This is the listener process top-level loop: wait for logging events
# (LogRecords)on the queue and handle them, quit when you get a None for a
# LogRecord.
def listener_process(queue, configurer):
    configurer()
    while True:
        try:
            record = queue.get()
            if record is None:  # We send this as a sentinel to tell the listener to quit.
                break
            logger = logging.getLogger(record.name)
            logger.handle(record)  # No level or filter logic applied - just do it!
        except Exception:
            import sys, traceback
            print('Whoops! Problem:', file=sys.stderr)
            traceback.print_exc(file=sys.stderr)

# Arrays used for random selections in this demo

LEVELS = [logging.DEBUG, logging.INFO, logging.WARNING,
          logging.ERROR, logging.CRITICAL]

LOGGERS = ['a.b.c', 'd.e.f']

MESSAGES = [
    'Random message #1',
    'Random message #2',
    'Random message #3',
]

# The worker configuration is done at the start of the worker process run.
# Note that on Windows you can't rely on fork semantics, so each process
# will run the logging configuration code when it starts.
def worker_configurer(queue):
    h = logging.handlers.QueueHandler(queue)  # Just the one handler needed
    root = logging.getLogger()
    root.addHandler(h)
    # send all messages, for demo; no other level or filter logic applied.
    root.setLevel(logging.DEBUG)

# This is the worker process top-level loop, which just logs ten events with
# random intervening delays before terminating.
# The print messages are just so you know it's doing something!
def worker_process(queue, configurer):
    configurer(queue)
    name = multiprocessing.current_process().name
    print('Worker started: %s' % name)
    for i in range(10):
        time.sleep(random())
        logger = logging.getLogger(choice(LOGGERS))
        level = choice(LEVELS)
        message = choice(MESSAGES)
        logger.log(level, message)
    print('Worker finished: %s' % name)

# Here's where the demo gets orchestrated. Create the queue, create and start
# the listener, create ten workers and start them, wait for them to finish,
# then send a None to the queue to tell the listener to finish.
def main():
    queue = multiprocessing.Queue(-1)
    listener = multiprocessing.Process(target=listener_process,
                                       args=(queue, listener_configurer))
    listener.start()
    workers = []
    for i in range(10):
        worker = multiprocessing.Process(target=worker_process,
                                         args=(queue, worker_configurer))
        workers.append(worker)
        worker.start()
    for w in workers:
        w.join()
    queue.put_nowait(None)
    listener.join()

if __name__ == '__main__':
    main()
</pre>
<p>A variant of the above script keeps the logging in the main process, in a
separate thread:</p>
<pre>import logging
import logging.config
import logging.handlers
from multiprocessing import Process, Queue
import random
import threading
import time

def logger_thread(q):
    while True:
        record = q.get()
        if record is None:
            break
        logger = logging.getLogger(record.name)
        logger.handle(record)


def worker_process(q):
    qh = logging.handlers.QueueHandler(q)
    root = logging.getLogger()
    root.setLevel(logging.DEBUG)
    root.addHandler(qh)
    levels = [logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR,
              logging.CRITICAL]
    loggers = ['foo', 'foo.bar', 'foo.bar.baz',
               'spam', 'spam.ham', 'spam.ham.eggs']
    for i in range(100):
        lvl = random.choice(levels)
        logger = logging.getLogger(random.choice(loggers))
        logger.log(lvl, 'Message no. %d', i)

if __name__ == '__main__':
    q = Queue()
    d = {
        'version': 1,
        'formatters': {
            'detailed': {
                'class': 'logging.Formatter',
                'format': '%(asctime)s %(name)-15s %(levelname)-8s %(processName)-10s %(message)s'
            }
        },
        'handlers': {
            'console': {
                'class': 'logging.StreamHandler',
                'level': 'INFO',
            },
            'file': {
                'class': 'logging.FileHandler',
                'filename': 'mplog.log',
                'mode': 'w',
                'formatter': 'detailed',
            },
            'foofile': {
                'class': 'logging.FileHandler',
                'filename': 'mplog-foo.log',
                'mode': 'w',
                'formatter': 'detailed',
            },
            'errors': {
                'class': 'logging.FileHandler',
                'filename': 'mplog-errors.log',
                'mode': 'w',
                'level': 'ERROR',
                'formatter': 'detailed',
            },
        },
        'loggers': {
            'foo': {
                'handlers': ['foofile']
            }
        },
        'root': {
            'level': 'DEBUG',
            'handlers': ['console', 'file', 'errors']
        },
    }
    workers = []
    for i in range(5):
        wp = Process(target=worker_process, name='worker %d' % (i + 1), args=(q,))
        workers.append(wp)
        wp.start()
    logging.config.dictConfig(d)
    lp = threading.Thread(target=logger_thread, args=(q,))
    lp.start()
    # At this point, the main process could do some useful work of its own
    # Once it's done that, it can wait for the workers to terminate...
    for wp in workers:
        wp.join()
    # And now tell the logging thread to finish up, too
    q.put(None)
    lp.join()
</pre>
<p>This variant shows how you can e.g. apply configuration for particular loggers
- e.g. the <code>foo</code> logger has a special handler which stores all events in the
<code>foo</code> subsystem in a file <code>mplog-foo.log</code>. This will be used by the logging
machinery in the main process (even though the logging events are generated in
the worker processes) to direct the messages to the appropriate destinations.</p>
<a name="user-content-using-file-rotation"></a>
<h2><a id="user-content-using-file-rotation" class="anchor" aria-hidden="true" href="#using-file-rotation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Using file rotation</h2>
<pre>.. sectionauthor:: Doug Hellmann, Vinay Sajip (changes)
</pre>
<p>Sometimes you want to let a log file grow to a certain size, then open a new
file and log to that. You may want to keep a certain number of these files, and
when that many files have been created, rotate the files so that the number of
files and the size of the files both remain bounded. For this usage pattern, the
logging package provides a <a href="#id98"><span id="user-content-id99">:class:`~handlers.RotatingFileHandler`</span></a>:</p>
<pre>import glob
import logging
import logging.handlers

LOG_FILENAME = 'logging_rotatingfile_example.out'

# Set up a specific logger with our desired output level
my_logger = logging.getLogger('MyLogger')
my_logger.setLevel(logging.DEBUG)

# Add the log message handler to the logger
handler = logging.handlers.RotatingFileHandler(
              LOG_FILENAME, maxBytes=20, backupCount=5)

my_logger.addHandler(handler)

# Log some messages
for i in range(20):
    my_logger.debug('i = %d' % i)

# See what files are created
logfiles = glob.glob('%s*' % LOG_FILENAME)

for filename in logfiles:
    print(filename)
</pre>
<p>The result should be 6 separate files, each with part of the log history for the
application:</p>
<pre lang="none">logging_rotatingfile_example.out
logging_rotatingfile_example.out.1
logging_rotatingfile_example.out.2
logging_rotatingfile_example.out.3
logging_rotatingfile_example.out.4
logging_rotatingfile_example.out.5
</pre>
<p>The most current file is always <a href="#id100"><span id="user-content-id101">:file:`logging_rotatingfile_example.out`</span></a>,
and each time it reaches the size limit it is renamed with the suffix
<code>.1</code>. Each of the existing backup files is renamed to increment the suffix
(<code>.1</code> becomes <code>.2</code>, etc.)  and the <code>.6</code> file is erased.</p>
<p>Obviously this example sets the log length much too small as an extreme
example.  You would want to set <em>maxBytes</em> to an appropriate value.</p>
<a name="user-content-use-of-alternative-formatting-styles"></a>
<h2><a id="user-content-use-of-alternative-formatting-styles" class="anchor" aria-hidden="true" href="#use-of-alternative-formatting-styles"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Use of alternative formatting styles</h2>
<p>When logging was added to the Python standard library, the only way of
formatting messages with variable content was to use the %-formatting
method. Since then, Python has gained two new formatting approaches:
<a href="#id102"><span id="user-content-id103">:class:`string.Template`</span></a> (added in Python 2.4) and <a href="#id104"><span id="user-content-id105">:meth:`str.format`</span></a>
(added in Python 2.6).</p>
<p>Logging (as of 3.2) provides improved support for these two additional
formatting styles. The <a href="#id106"><span id="user-content-id107">:class:`Formatter`</span></a> class been enhanced to take an
additional, optional keyword parameter named <code>style</code>. This defaults to
<code>'%'</code>, but other possible values are <code>'{'</code> and <code>'$'</code>, which correspond
to the other two formatting styles. Backwards compatibility is maintained by
default (as you would expect), but by explicitly specifying a style parameter,
you get the ability to specify format strings which work with
<a href="#id108"><span id="user-content-id109">:meth:`str.format`</span></a> or <a href="#id110"><span id="user-content-id111">:class:`string.Template`</span></a>. Here's an example console
session to show the possibilities:</p>
<div class="highlight highlight-text-python-console"><pre>&gt;&gt;&gt; <span class="pl-k">import</span> logging
&gt;&gt;&gt; root <span class="pl-k">=</span> logging.getLogger()
&gt;&gt;&gt; root.setLevel(logging.<span class="pl-c1">DEBUG</span>)
&gt;&gt;&gt; handler <span class="pl-k">=</span> logging.StreamHandler()
&gt;&gt;&gt; bf <span class="pl-k">=</span> logging.Formatter(<span class="pl-s"><span class="pl-pds">'</span><span class="pl-c1">{asctime}</span> <span class="pl-c1">{name}</span> <span class="pl-c1">{levelname<span class="pl-k">:8s</span>}</span> <span class="pl-c1">{message}</span><span class="pl-pds">'</span></span>,
...                        style<span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">'</span>{<span class="pl-pds">'</span></span>)
&gt;&gt;&gt; handler.setFormatter(bf)
&gt;&gt;&gt; root.addHandler(handler)
&gt;&gt;&gt; logger <span class="pl-k">=</span> logging.getLogger(<span class="pl-s"><span class="pl-pds">'</span>foo.bar<span class="pl-pds">'</span></span>)
&gt;&gt;&gt; logger.debug(<span class="pl-s"><span class="pl-pds">'</span>This is a DEBUG message<span class="pl-pds">'</span></span>)
2010-10-28 15:11:55,341 foo.bar DEBUG    This is a DEBUG message
&gt;&gt;&gt; logger.critical(<span class="pl-s"><span class="pl-pds">'</span>This is a CRITICAL message<span class="pl-pds">'</span></span>)
2010-10-28 15:12:11,526 foo.bar CRITICAL This is a CRITICAL message
&gt;&gt;&gt; df <span class="pl-k">=</span> logging.Formatter(<span class="pl-s"><span class="pl-pds">'</span>$asctime $name $<span class="pl-c1">{levelname}</span> $message<span class="pl-pds">'</span></span>,
...                        style<span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">'</span>$<span class="pl-pds">'</span></span>)
&gt;&gt;&gt; handler.setFormatter(df)
&gt;&gt;&gt; logger.debug(<span class="pl-s"><span class="pl-pds">'</span>This is a DEBUG message<span class="pl-pds">'</span></span>)
2010-10-28 15:13:06,924 foo.bar DEBUG This is a DEBUG message
&gt;&gt;&gt; logger.critical(<span class="pl-s"><span class="pl-pds">'</span>This is a CRITICAL message<span class="pl-pds">'</span></span>)
2010-10-28 15:13:11,494 foo.bar CRITICAL This is a CRITICAL message
&gt;&gt;&gt;</pre></div>
<p>Note that the formatting of logging messages for final output to logs is
completely independent of how an individual logging message is constructed.
That can still use %-formatting, as shown here:</p>
<pre>&gt;&gt;&gt; logger.error('This is an%s %s %s', 'other,', 'ERROR,', 'message')
2010-10-28 15:19:29,833 foo.bar ERROR This is another, ERROR, message
&gt;&gt;&gt;
</pre>
<p>Logging calls (<code>logger.debug()</code>, <code>logger.info()</code> etc.) only take
positional parameters for the actual logging message itself, with keyword
parameters used only for determining options for how to handle the actual
logging call (e.g. the <code>exc_info</code> keyword parameter to indicate that
traceback information should be logged, or the <code>extra</code> keyword parameter
to indicate additional contextual information to be added to the log). So
you cannot directly make logging calls using <a href="#id112"><span id="user-content-id113">:meth:`str.format`</span></a> or
<a href="#id114"><span id="user-content-id115">:class:`string.Template`</span></a> syntax, because internally the logging package
uses %-formatting to merge the format string and the variable arguments.
There would be no changing this while preserving backward compatibility, since
all logging calls which are out there in existing code will be using %-format
strings.</p>
<p>There is, however, a way that you can use {}- and $- formatting to construct
your individual log messages. Recall that for a message you can use an
arbitrary object as a message format string, and that the logging package will
call <code>str()</code> on that object to get the actual format string. Consider the
following two classes:</p>
<pre>class BraceMessage:
    def __init__(self, fmt, *args, **kwargs):
        self.fmt = fmt
        self.args = args
        self.kwargs = kwargs

    def __str__(self):
        return self.fmt.format(*self.args, **self.kwargs)

class DollarMessage:
    def __init__(self, fmt, **kwargs):
        self.fmt = fmt
        self.kwargs = kwargs

    def __str__(self):
        from string import Template
        return Template(self.fmt).substitute(**self.kwargs)
</pre>
<p>Either of these can be used in place of a format string, to allow {}- or
$-formatting to be used to build the actual "message" part which appears in the
formatted log output in place of "%(message)s" or "{message}" or "$message".
It's a little unwieldy to use the class names whenever you want to log
something, but it's quite palatable if you use an alias such as __ (double
underscore --- not to be confused with _, the single underscore used as a
synonym/alias for <a href="#id116"><span id="user-content-id117">:func:`gettext.gettext`</span></a> or its brethren).</p>
<p>The above classes are not included in Python, though they're easy enough to
copy and paste into your own code. They can be used as follows (assuming that
they're declared in a module called <code>wherever</code>):</p>
<div class="highlight highlight-text-python-console"><pre>&gt;&gt;&gt; <span class="pl-k">from</span> wherever <span class="pl-k">import</span> BraceMessage <span class="pl-k">as</span> __
&gt;&gt;&gt; <span class="pl-c1">print</span>(__(<span class="pl-s"><span class="pl-pds">'</span>Message with <span class="pl-c1">{0}</span> <span class="pl-c1">{name}</span><span class="pl-pds">'</span></span>, <span class="pl-c1">2</span>, <span class="pl-v">name</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">'</span>placeholders<span class="pl-pds">'</span></span>))
Message with 2 placeholders
&gt;&gt;&gt; <span class="pl-k">class</span> <span class="pl-en">Point</span>: <span class="pl-k">pass</span>
...
&gt;&gt;&gt; p <span class="pl-k">=</span> Point()
&gt;&gt;&gt; p.x <span class="pl-k">=</span> <span class="pl-c1">0.5</span>
&gt;&gt;&gt; p.y <span class="pl-k">=</span> <span class="pl-c1">0.5</span>
&gt;&gt;&gt; <span class="pl-c1">print</span>(__(<span class="pl-s"><span class="pl-pds">'</span>Message with coordinates: (<span class="pl-c1">{point.x<span class="pl-k">:.2f</span>}</span>, <span class="pl-c1">{point.y<span class="pl-k">:.2f</span>}</span>)<span class="pl-pds">'</span></span>,
...       point<span class="pl-k">=</span>p))
Message with coordinates: (0.50, 0.50)
&gt;&gt;&gt; <span class="pl-k">from</span> wherever <span class="pl-k">import</span> DollarMessage <span class="pl-k">as</span> __
&gt;&gt;&gt; <span class="pl-c1">print</span>(__(<span class="pl-s"><span class="pl-pds">'</span>Message with $num $what<span class="pl-pds">'</span></span>, <span class="pl-v">num</span><span class="pl-k">=</span><span class="pl-c1">2</span>, <span class="pl-v">what</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">'</span>placeholders<span class="pl-pds">'</span></span>))
Message with 2 placeholders
&gt;&gt;&gt;</pre></div>
<p>While the above examples use <code>print()</code> to show how the formatting works, you
would of course use <code>logger.debug()</code> or similar to actually log using this
approach.</p>
<p>One thing to note is that you pay no significant performance penalty with this
approach: the actual formatting happens not when you make the logging call, but
when (and if) the logged message is actually about to be output to a log by a
handler. So the only slightly unusual thing which might trip you up is that the
parentheses go around the format string and the arguments, not just the format
string. That's because the __ notation is just syntax sugar for a constructor
call to one of the XXXMessage classes.</p>
<p>If you prefer, you can use a <a href="#id118"><span id="user-content-id119">:class:`LoggerAdapter`</span></a> to achieve a similar effect
to the above, as in the following example:</p>
<pre>import logging

class Message(object):
    def __init__(self, fmt, args):
        self.fmt = fmt
        self.args = args

    def __str__(self):
        return self.fmt.format(*self.args)

class StyleAdapter(logging.LoggerAdapter):
    def __init__(self, logger, extra=None):
        super(StyleAdapter, self).__init__(logger, extra or {})

    def log(self, level, msg, *args, **kwargs):
        if self.isEnabledFor(level):
            msg, kwargs = self.process(msg, kwargs)
            self.logger._log(level, Message(msg, args), (), **kwargs)

logger = StyleAdapter(logging.getLogger(__name__))

def main():
    logger.debug('Hello, {}', 'world!')

if __name__ == '__main__':
    logging.basicConfig(level=logging.DEBUG)
    main()
</pre>
<p>The above script should log the message <code>Hello, world!</code> when run with
Python 3.2 or later.</p>
<pre>.. currentmodule:: logging

</pre>
<a name="user-content-customizing-logrecord"></a>
<h2><a id="user-content-customizing-logrecord" class="anchor" aria-hidden="true" href="#customizing-logrecord"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Customizing <code>LogRecord</code></h2>
<p>Every logging event is represented by a <a href="#id120"><span id="user-content-id121">:class:`LogRecord`</span></a> instance.
When an event is logged and not filtered out by a logger's level, a
<a href="#id122"><span id="user-content-id123">:class:`LogRecord`</span></a> is created, populated with information about the event and
then passed to the handlers for that logger (and its ancestors, up to and
including the logger where further propagation up the hierarchy is disabled).
Before Python 3.2, there were only two places where this creation was done:</p>
<ul>
<li><a href="#id124"><span id="user-content-id125">:meth:`Logger.makeRecord`</span></a>, which is called in the normal process of
logging an event. This invoked <a href="#id126"><span id="user-content-id127">:class:`LogRecord`</span></a> directly to create an
instance.</li>
<li><a href="#id128"><span id="user-content-id129">:func:`makeLogRecord`</span></a>, which is called with a dictionary containing
attributes to be added to the LogRecord. This is typically invoked when a
suitable dictionary has been received over the network (e.g. in pickle form
via a <a href="#id130"><span id="user-content-id131">:class:`~handlers.SocketHandler`</span></a>, or in JSON form via an
<a href="#id132"><span id="user-content-id133">:class:`~handlers.HTTPHandler`</span></a>).</li>
</ul>
<p>This has usually meant that if you need to do anything special with a
<a href="#id134"><span id="user-content-id135">:class:`LogRecord`</span></a>, you've had to do one of the following.</p>
<ul>
<li>Create your own <a href="#id136"><span id="user-content-id137">:class:`Logger`</span></a> subclass, which overrides
<a href="#id138"><span id="user-content-id139">:meth:`Logger.makeRecord`</span></a>, and set it using <a href="#id140"><span id="user-content-id141">:func:`~logging.setLoggerClass`</span></a>
before any loggers that you care about are instantiated.</li>
<li>Add a <a href="#id142"><span id="user-content-id143">:class:`Filter`</span></a> to a logger or handler, which does the
necessary special manipulation you need when its
<a href="#id144"><span id="user-content-id145">:meth:`~Filter.filter`</span></a> method is called.</li>
</ul>
<p>The first approach would be a little unwieldy in the scenario where (say)
several different libraries wanted to do different things. Each would attempt
to set its own <a href="#id146"><span id="user-content-id147">:class:`Logger`</span></a> subclass, and the one which did this last would
win.</p>
<p>The second approach works reasonably well for many cases, but does not allow
you to e.g. use a specialized subclass of <a href="#id148"><span id="user-content-id149">:class:`LogRecord`</span></a>. Library
developers can set a suitable filter on their loggers, but they would have to
remember to do this every time they introduced a new logger (which they would
do simply by adding new packages or modules and doing</p>
<pre>logger = logging.getLogger(__name__)
</pre>
<p>at module level). It's probably one too many things to think about. Developers
could also add the filter to a <a href="#id150"><span id="user-content-id151">:class:`~logging.NullHandler`</span></a> attached to their
top-level logger, but this would not be invoked if an application developer
attached a handler to a lower-level library logger --- so output from that
handler would not reflect the intentions of the library developer.</p>
<p>In Python 3.2 and later, <a href="#id152"><span id="user-content-id153">:class:`~logging.LogRecord`</span></a> creation is done through a
factory, which you can specify. The factory is just a callable you can set with
<a href="#id154"><span id="user-content-id155">:func:`~logging.setLogRecordFactory`</span></a>, and interrogate with
<a href="#id156"><span id="user-content-id157">:func:`~logging.getLogRecordFactory`</span></a>. The factory is invoked with the same
signature as the <a href="#id158"><span id="user-content-id159">:class:`~logging.LogRecord`</span></a> constructor, as <a href="#id160"><span id="user-content-id161">:class:`LogRecord`</span></a>
is the default setting for the factory.</p>
<p>This approach allows a custom factory to control all aspects of LogRecord
creation. For example, you could return a subclass, or just add some additional
attributes to the record once created, using a pattern similar to this:</p>
<pre>old_factory = logging.getLogRecordFactory()

def record_factory(*args, **kwargs):
    record = old_factory(*args, **kwargs)
    record.custom_attribute = 0xdecafbad
    return record

logging.setLogRecordFactory(record_factory)
</pre>
<p>This pattern allows different libraries to chain factories together, and as
long as they don't overwrite each other's attributes or unintentionally
overwrite the attributes provided as standard, there should be no surprises.
However, it should be borne in mind that each link in the chain adds run-time
overhead to all logging operations, and the technique should only be used when
the use of a <a href="#id162"><span id="user-content-id163">:class:`Filter`</span></a> does not provide the desired result.</p>
<a name="user-content-subclassing-queuehandler-a-zeromq-example"></a>
<h2><a id="user-content-subclassing-queuehandler---a-zeromq-example" class="anchor" aria-hidden="true" href="#subclassing-queuehandler---a-zeromq-example"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Subclassing QueueHandler - a ZeroMQ example</h2>
<p>You can use a <a href="#id164"><span id="user-content-id165">:class:`QueueHandler`</span></a> subclass to send messages to other kinds
of queues, for example a ZeroMQ 'publish' socket. In the example below,the
socket is created separately and passed to the handler (as its 'queue'):</p>
<pre>import zmq   # using pyzmq, the Python binding for ZeroMQ
import json  # for serializing records portably

ctx = zmq.Context()
sock = zmq.Socket(ctx, zmq.PUB)  # or zmq.PUSH, or other suitable value
sock.bind('tcp://*:5556')        # or wherever

class ZeroMQSocketHandler(QueueHandler):
    def enqueue(self, record):
        self.queue.send_json(record.__dict__)


handler = ZeroMQSocketHandler(sock)
</pre>
<p>Of course there are other ways of organizing this, for example passing in the
data needed by the handler to create the socket:</p>
<pre>class ZeroMQSocketHandler(QueueHandler):
    def __init__(self, uri, socktype=zmq.PUB, ctx=None):
        self.ctx = ctx or zmq.Context()
        socket = zmq.Socket(self.ctx, socktype)
        socket.bind(uri)
        super().__init__(socket)

    def enqueue(self, record):
        self.queue.send_json(record.__dict__)

    def close(self):
        self.queue.close()
</pre>
<a name="user-content-subclassing-queuelistener-a-zeromq-example"></a>
<h2><a id="user-content-subclassing-queuelistener---a-zeromq-example" class="anchor" aria-hidden="true" href="#subclassing-queuelistener---a-zeromq-example"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Subclassing QueueListener - a ZeroMQ example</h2>
<p>You can also subclass <a href="#id166"><span id="user-content-id167">:class:`QueueListener`</span></a> to get messages from other kinds
of queues, for example a ZeroMQ 'subscribe' socket. Here's an example:</p>
<pre>class ZeroMQSocketListener(QueueListener):
    def __init__(self, uri, *handlers, **kwargs):
        self.ctx = kwargs.get('ctx') or zmq.Context()
        socket = zmq.Socket(self.ctx, zmq.SUB)
        socket.setsockopt_string(zmq.SUBSCRIBE, '')  # subscribe to everything
        socket.connect(uri)
        super().__init__(socket, *handlers, **kwargs)

    def dequeue(self):
        msg = self.queue.recv_json()
        return logging.makeLogRecord(msg)
</pre>
<pre>.. seealso::

   Module :mod:`logging`
      API reference for the logging module.

   Module :mod:`logging.config`
      Configuration API for the logging module.

   Module :mod:`logging.handlers`
      Useful handlers included with the logging module.

   :ref:`A basic logging tutorial &lt;logging-basic-tutorial&gt;`

   :ref:`A more advanced logging tutorial &lt;logging-advanced-tutorial&gt;`


</pre>
<a name="user-content-an-example-dictionary-based-configuration"></a>
<h2><a id="user-content-an-example-dictionary-based-configuration" class="anchor" aria-hidden="true" href="#an-example-dictionary-based-configuration"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>An example dictionary-based configuration</h2>
<p>Below is an example of a logging configuration dictionary - it's taken from
the <a href="https://docs.djangoproject.com/en/1.9/topics/logging/#configuring-logging" rel="nofollow">documentation on the Django project</a>.
This dictionary is passed to <a href="#id168"><span id="user-content-id169">:func:`~config.dictConfig`</span></a> to put the configuration into effect:</p>
<pre>LOGGING = {
    'version': 1,
    'disable_existing_loggers': True,
    'formatters': {
        'verbose': {
            'format': '%(levelname)s %(asctime)s %(module)s %(process)d %(thread)d %(message)s'
        },
        'simple': {
            'format': '%(levelname)s %(message)s'
        },
    },
    'filters': {
        'special': {
            '()': 'project.logging.SpecialFilter',
            'foo': 'bar',
        }
    },
    'handlers': {
        'null': {
            'level':'DEBUG',
            'class':'django.utils.log.NullHandler',
        },
        'console':{
            'level':'DEBUG',
            'class':'logging.StreamHandler',
            'formatter': 'simple'
        },
        'mail_admins': {
            'level': 'ERROR',
            'class': 'django.utils.log.AdminEmailHandler',
            'filters': ['special']
        }
    },
    'loggers': {
        'django': {
            'handlers':['null'],
            'propagate': True,
            'level':'INFO',
        },
        'django.request': {
            'handlers': ['mail_admins'],
            'level': 'ERROR',
            'propagate': False,
        },
        'myproject.custom': {
            'handlers': ['console', 'mail_admins'],
            'level': 'INFO',
            'filters': ['special']
        }
    }
}
</pre>
<p>For more information about this configuration, you can see the <a href="https://docs.djangoproject.com/en/1.9/topics/logging/#configuring-logging" rel="nofollow">relevant
section</a>
of the Django documentation.</p>
<a name="user-content-using-a-rotator-and-namer-to-customize-log-rotation-processing"></a>
<h2><a id="user-content-using-a-rotator-and-namer-to-customize-log-rotation-processing" class="anchor" aria-hidden="true" href="#using-a-rotator-and-namer-to-customize-log-rotation-processing"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Using a rotator and namer to customize log rotation processing</h2>
<p>An example of how you can define a namer and rotator is given in the following
snippet, which shows zlib-based compression of the log file:</p>
<pre>def namer(name):
    return name + ".gz"

def rotator(source, dest):
    with open(source, "rb") as sf:
        data = sf.read()
        compressed = zlib.compress(data, 9)
        with open(dest, "wb") as df:
            df.write(compressed)
    os.remove(source)

rh = logging.handlers.RotatingFileHandler(...)
rh.rotator = rotator
rh.namer = namer
</pre>
<p>These are not "true" .gz files, as they are bare compressed data, with no
"container" such as you’d find in an actual gzip file. This snippet is just
for illustration purposes.</p>
<a name="user-content-a-more-elaborate-multiprocessing-example"></a>
<h2><a id="user-content-a-more-elaborate-multiprocessing-example" class="anchor" aria-hidden="true" href="#a-more-elaborate-multiprocessing-example"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>A more elaborate multiprocessing example</h2>
<p>The following working example shows how logging can be used with multiprocessing
using configuration files. The configurations are fairly simple, but serve to
illustrate how more complex ones could be implemented in a real multiprocessing
scenario.</p>
<p>In the example, the main process spawns a listener process and some worker
processes. Each of the main process, the listener and the workers have three
separate configurations (the workers all share the same configuration). We can
see logging in the main process, how the workers log to a QueueHandler and how
the listener implements a QueueListener and a more complex logging
configuration, and arranges to dispatch events received via the queue to the
handlers specified in the configuration. Note that these configurations are
purely illustrative, but you should be able to adapt this example to your own
scenario.</p>
<p>Here's the script - the docstrings and the comments hopefully explain how it
works:</p>
<pre>import logging
import logging.config
import logging.handlers
from multiprocessing import Process, Queue, Event, current_process
import os
import random
import time

class MyHandler:
    """
    A simple handler for logging events. It runs in the listener process and
    dispatches events to loggers based on the name in the received record,
    which then get dispatched, by the logging system, to the handlers
    configured for those loggers.
    """

    def handle(self, record):
        if record.name == "root":
            logger = logging.getLogger()
        else:
            logger = logging.getLogger(record.name)

        if logger.isEnabledFor(record.levelno):
            # The process name is transformed just to show that it's the listener
            # doing the logging to files and console
            record.processName = '%s (for %s)' % (current_process().name, record.processName)
            logger.handle(record)

def listener_process(q, stop_event, config):
    """
    This could be done in the main process, but is just done in a separate
    process for illustrative purposes.

    This initialises logging according to the specified configuration,
    starts the listener and waits for the main process to signal completion
    via the event. The listener is then stopped, and the process exits.
    """
    logging.config.dictConfig(config)
    listener = logging.handlers.QueueListener(q, MyHandler())
    listener.start()
    if os.name == 'posix':
        # On POSIX, the setup logger will have been configured in the
        # parent process, but should have been disabled following the
        # dictConfig call.
        # On Windows, since fork isn't used, the setup logger won't
        # exist in the child, so it would be created and the message
        # would appear - hence the "if posix" clause.
        logger = logging.getLogger('setup')
        logger.critical('Should not appear, because of disabled logger ...')
    stop_event.wait()
    listener.stop()

def worker_process(config):
    """
    A number of these are spawned for the purpose of illustration. In
    practice, they could be a heterogeneous bunch of processes rather than
    ones which are identical to each other.

    This initialises logging according to the specified configuration,
    and logs a hundred messages with random levels to randomly selected
    loggers.

    A small sleep is added to allow other processes a chance to run. This
    is not strictly needed, but it mixes the output from the different
    processes a bit more than if it's left out.
    """
    logging.config.dictConfig(config)
    levels = [logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR,
              logging.CRITICAL]
    loggers = ['foo', 'foo.bar', 'foo.bar.baz',
               'spam', 'spam.ham', 'spam.ham.eggs']
    if os.name == 'posix':
        # On POSIX, the setup logger will have been configured in the
        # parent process, but should have been disabled following the
        # dictConfig call.
        # On Windows, since fork isn't used, the setup logger won't
        # exist in the child, so it would be created and the message
        # would appear - hence the "if posix" clause.
        logger = logging.getLogger('setup')
        logger.critical('Should not appear, because of disabled logger ...')
    for i in range(100):
        lvl = random.choice(levels)
        logger = logging.getLogger(random.choice(loggers))
        logger.log(lvl, 'Message no. %d', i)
        time.sleep(0.01)

def main():
    q = Queue()
    # The main process gets a simple configuration which prints to the console.
    config_initial = {
        'version': 1,
        'handlers': {
            'console': {
                'class': 'logging.StreamHandler',
                'level': 'INFO'
            }
        },
        'root': {
            'handlers': ['console'],
            'level': 'DEBUG'
        }
    }
    # The worker process configuration is just a QueueHandler attached to the
    # root logger, which allows all messages to be sent to the queue.
    # We disable existing loggers to disable the "setup" logger used in the
    # parent process. This is needed on POSIX because the logger will
    # be there in the child following a fork().
    config_worker = {
        'version': 1,
        'disable_existing_loggers': True,
        'handlers': {
            'queue': {
                'class': 'logging.handlers.QueueHandler',
                'queue': q
            }
        },
        'root': {
            'handlers': ['queue'],
            'level': 'DEBUG'
        }
    }
    # The listener process configuration shows that the full flexibility of
    # logging configuration is available to dispatch events to handlers however
    # you want.
    # We disable existing loggers to disable the "setup" logger used in the
    # parent process. This is needed on POSIX because the logger will
    # be there in the child following a fork().
    config_listener = {
        'version': 1,
        'disable_existing_loggers': True,
        'formatters': {
            'detailed': {
                'class': 'logging.Formatter',
                'format': '%(asctime)s %(name)-15s %(levelname)-8s %(processName)-10s %(message)s'
            },
            'simple': {
                'class': 'logging.Formatter',
                'format': '%(name)-15s %(levelname)-8s %(processName)-10s %(message)s'
            }
        },
        'handlers': {
            'console': {
                'class': 'logging.StreamHandler',
                'formatter': 'simple',
                'level': 'INFO'
            },
            'file': {
                'class': 'logging.FileHandler',
                'filename': 'mplog.log',
                'mode': 'w',
                'formatter': 'detailed'
            },
            'foofile': {
                'class': 'logging.FileHandler',
                'filename': 'mplog-foo.log',
                'mode': 'w',
                'formatter': 'detailed'
            },
            'errors': {
                'class': 'logging.FileHandler',
                'filename': 'mplog-errors.log',
                'mode': 'w',
                'formatter': 'detailed',
                'level': 'ERROR'
            }
        },
        'loggers': {
            'foo': {
                'handlers': ['foofile']
            }
        },
        'root': {
            'handlers': ['console', 'file', 'errors'],
            'level': 'DEBUG'
        }
    }
    # Log some initial events, just to show that logging in the parent works
    # normally.
    logging.config.dictConfig(config_initial)
    logger = logging.getLogger('setup')
    logger.info('About to create workers ...')
    workers = []
    for i in range(5):
        wp = Process(target=worker_process, name='worker %d' % (i + 1),
                     args=(config_worker,))
        workers.append(wp)
        wp.start()
        logger.info('Started worker: %s', wp.name)
    logger.info('About to create listener ...')
    stop_event = Event()
    lp = Process(target=listener_process, name='listener',
                 args=(q, stop_event, config_listener))
    lp.start()
    logger.info('Started listener')
    # We now hang around for the workers to finish their work.
    for wp in workers:
        wp.join()
    # Workers all done, listening can now stop.
    # Logging in the parent still works normally.
    logger.info('Telling listener to stop ...')
    stop_event.set()
    lp.join()
    logger.info('All done.')

if __name__ == '__main__':
    main()
</pre>
<a name="user-content-inserting-a-bom-into-messages-sent-to-a-sysloghandler"></a>
<h2><a id="user-content-inserting-a-bom-into-messages-sent-to-a-sysloghandler" class="anchor" aria-hidden="true" href="#inserting-a-bom-into-messages-sent-to-a-sysloghandler"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Inserting a BOM into messages sent to a SysLogHandler</h2>
<p><a href="http://tools.ietf.org/html/rfc5424.html" rel="nofollow">RFC 5424</a> requires that a
Unicode message be sent to a syslog daemon as a set of bytes which have the
following structure: an optional pure-ASCII component, followed by a UTF-8 Byte
Order Mark (BOM), followed by Unicode encoded using UTF-8. (See the
<a href="#id170"><span id="user-content-id171">:rfc:`relevant section of the specification &lt;5424#section-6&gt;`</span></a>.)</p>
<p>In Python 3.1, code was added to
<a href="#id172"><span id="user-content-id173">:class:`~logging.handlers.SysLogHandler`</span></a> to insert a BOM into the message, but
unfortunately, it was implemented incorrectly, with the BOM appearing at the
beginning of the message and hence not allowing any pure-ASCII component to
appear before it.</p>
<p>As this behaviour is broken, the incorrect BOM insertion code is being removed
from Python 3.2.4 and later. However, it is not being replaced, and if you
want to produce <a href="http://tools.ietf.org/html/rfc5424.html" rel="nofollow">RFC 5424</a>-compliant messages which include a BOM, an optional
pure-ASCII sequence before it and arbitrary Unicode after it, encoded using
UTF-8, then you need to do the following:</p>
<ol>
<li><p>Attach a <a href="#id174"><span id="user-content-id175">:class:`~logging.Formatter`</span></a> instance to your
<a href="#id176"><span id="user-content-id177">:class:`~logging.handlers.SysLogHandler`</span></a> instance, with a format string
such as:</p>
<pre>'ASCII section\ufeffUnicode section'
</pre>
<p>The Unicode code point U+FEFF, when encoded using UTF-8, will be
encoded as a UTF-8 BOM -- the byte-string <code>b'\xef\xbb\xbf'</code>.</p>
</li>
<li><p>Replace the ASCII section with whatever placeholders you like, but make sure
that the data that appears in there after substitution is always ASCII (that
way, it will remain unchanged after UTF-8 encoding).</p>
</li>
<li><p>Replace the Unicode section with whatever placeholders you like; if the data
which appears there after substitution contains characters outside the ASCII
range, that's fine -- it will be encoded using UTF-8.</p>
</li>
</ol>
<p>The formatted message <em>will</em> be encoded using UTF-8 encoding by
<code>SysLogHandler</code>. If you follow the above rules, you should be able to produce
<a href="http://tools.ietf.org/html/rfc5424.html" rel="nofollow">RFC 5424</a>-compliant messages. If you don't, logging may not complain, but your
messages will not be RFC 5424-compliant, and your syslog daemon may complain.</p>
<a name="user-content-implementing-structured-logging"></a>
<h2><a id="user-content-implementing-structured-logging" class="anchor" aria-hidden="true" href="#implementing-structured-logging"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Implementing structured logging</h2>
<p>Although most logging messages are intended for reading by humans, and thus not
readily machine-parseable, there might be circumstances where you want to output
messages in a structured format which <em>is</em> capable of being parsed by a program
(without needing complex regular expressions to parse the log message). This is
straightforward to achieve using the logging package. There are a number of
ways in which this could be achieved, but the following is a simple approach
which uses JSON to serialise the event in a machine-parseable manner:</p>
<pre>import json
import logging

class StructuredMessage(object):
    def __init__(self, message, **kwargs):
        self.message = message
        self.kwargs = kwargs

    def __str__(self):
        return '%s &gt;&gt;&gt; %s' % (self.message, json.dumps(self.kwargs))

_ = StructuredMessage   # optional, to improve readability

logging.basicConfig(level=logging.INFO, format='%(message)s')
logging.info(_('message 1', foo='bar', bar='baz', num=123, fnum=123.456))
</pre>
<p>If the above script is run, it prints:</p>
<pre lang="none">message 1 &gt;&gt;&gt; {"fnum": 123.456, "num": 123, "bar": "baz", "foo": "bar"}
</pre>
<p>Note that the order of items might be different according to the version of
Python used.</p>
<p>If you need more specialised processing, you can use a custom JSON encoder,
as in the following complete example:</p>
<pre>from __future__ import unicode_literals

import json
import logging

# This next bit is to ensure the script runs unchanged on 2.x and 3.x
try:
    unicode
except NameError:
    unicode = str

class Encoder(json.JSONEncoder):
    def default(self, o):
        if isinstance(o, set):
            return tuple(o)
        elif isinstance(o, unicode):
            return o.encode('unicode_escape').decode('ascii')
        return super(Encoder, self).default(o)

class StructuredMessage(object):
    def __init__(self, message, **kwargs):
        self.message = message
        self.kwargs = kwargs

    def __str__(self):
        s = Encoder().encode(self.kwargs)
        return '%s &gt;&gt;&gt; %s' % (self.message, s)

_ = StructuredMessage   # optional, to improve readability

def main():
    logging.basicConfig(level=logging.INFO, format='%(message)s')
    logging.info(_('message 1', set_value={1, 2, 3}, snowman='\u2603'))

if __name__ == '__main__':
    main()
</pre>
<p>When the above script is run, it prints:</p>
<pre lang="none">message 1 &gt;&gt;&gt; {"snowman": "\u2603", "set_value": [1, 2, 3]}
</pre>
<p>Note that the order of items might be different according to the version of
Python used.</p>
<pre>.. currentmodule:: logging.config

</pre>
<a name="user-content-customizing-handlers-with-func-dictconfig"></a>
<h2><a id="user-content-customizing-handlers-with-funcdictconfig" class="anchor" aria-hidden="true" href="#customizing-handlers-with-funcdictconfig"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Customizing handlers with <a href="#id178"><span id="user-content-id179">:func:`dictConfig`</span></a></h2>
<p>There are times when you want to customize logging handlers in particular ways,
and if you use <a href="#id180"><span id="user-content-id181">:func:`dictConfig`</span></a> you may be able to do this without
subclassing. As an example, consider that you may want to set the ownership of a
log file. On POSIX, this is easily done using <a href="#id182"><span id="user-content-id183">:func:`shutil.chown`</span></a>, but the file
handlers in the stdlib don't offer built-in support. You can customize handler
creation using a plain function such as:</p>
<pre>def owned_file_handler(filename, mode='a', encoding=None, owner=None):
    if owner:
        if not os.path.exists(filename):
            open(filename, 'a').close()
        shutil.chown(filename, *owner)
    return logging.FileHandler(filename, mode, encoding)
</pre>
<p>You can then specify, in a logging configuration passed to <a href="#id184"><span id="user-content-id185">:func:`dictConfig`</span></a>,
that a logging handler be created by calling this function:</p>
<pre>LOGGING = {
    'version': 1,
    'disable_existing_loggers': False,
    'formatters': {
        'default': {
            'format': '%(asctime)s %(levelname)s %(name)s %(message)s'
        },
    },
    'handlers': {
        'file':{
            # The values below are popped from this dictionary and
            # used to create the handler, set the handler's level and
            # its formatter.
            '()': owned_file_handler,
            'level':'DEBUG',
            'formatter': 'default',
            # The values below are passed to the handler creator callable
            # as keyword arguments.
            'owner': ['pulse', 'pulse'],
            'filename': 'chowntest.log',
            'mode': 'w',
            'encoding': 'utf-8',
        },
    },
    'root': {
        'handlers': ['file'],
        'level': 'DEBUG',
    },
}
</pre>
<p>In this example I am setting the ownership using the <code>pulse</code> user and group,
just for the purposes of illustration. Putting it together into a working
script, <code>chowntest.py</code>:</p>
<pre>import logging, logging.config, os, shutil

def owned_file_handler(filename, mode='a', encoding=None, owner=None):
    if owner:
        if not os.path.exists(filename):
            open(filename, 'a').close()
        shutil.chown(filename, *owner)
    return logging.FileHandler(filename, mode, encoding)

LOGGING = {
    'version': 1,
    'disable_existing_loggers': False,
    'formatters': {
        'default': {
            'format': '%(asctime)s %(levelname)s %(name)s %(message)s'
        },
    },
    'handlers': {
        'file':{
            # The values below are popped from this dictionary and
            # used to create the handler, set the handler's level and
            # its formatter.
            '()': owned_file_handler,
            'level':'DEBUG',
            'formatter': 'default',
            # The values below are passed to the handler creator callable
            # as keyword arguments.
            'owner': ['pulse', 'pulse'],
            'filename': 'chowntest.log',
            'mode': 'w',
            'encoding': 'utf-8',
        },
    },
    'root': {
        'handlers': ['file'],
        'level': 'DEBUG',
    },
}

logging.config.dictConfig(LOGGING)
logger = logging.getLogger('mylogger')
logger.debug('A debug message')
</pre>
<p>To run this, you will probably need to run as <code>root</code>:</p>
<pre lang="shell-session">$ sudo python3.3 chowntest.py
$ cat chowntest.log
2013-11-05 09:34:51,128 DEBUG mylogger A debug message
$ ls -l chowntest.log
-rw-r--r-- 1 pulse pulse 55 2013-11-05 09:34 chowntest.log
</pre>
<p>Note that this example uses Python 3.3 because that's where <a href="#id186"><span id="user-content-id187">:func:`shutil.chown`</span></a>
makes an appearance. This approach should work with any Python version that
supports <a href="#id188"><span id="user-content-id189">:func:`dictConfig`</span></a> - namely, Python 2.7, 3.2 or later. With pre-3.3
versions, you would need to implement the actual ownership change using e.g.
<a href="#id190"><span id="user-content-id191">:func:`os.chown`</span></a>.</p>
<p>In practice, the handler-creating function may be in a utility module somewhere
in your project. Instead of the line in the configuration:</p>
<pre>'()': owned_file_handler,
</pre>
<p>you could use e.g.:</p>
<pre>'()': 'ext://project.util.owned_file_handler',
</pre>
<p>where <code>project.util</code> can be replaced with the actual name of the package
where the function resides. In the above working script, using
<code>'ext://__main__.owned_file_handler'</code> should work. Here, the actual callable
is resolved by <a href="#id192"><span id="user-content-id193">:func:`dictConfig`</span></a> from the <code>ext://</code> specification.</p>
<p>This example hopefully also points the way to how you could implement other
types of file change - e.g. setting specific POSIX permission bits - in the
same way, using <a href="#id194"><span id="user-content-id195">:func:`os.chmod`</span></a>.</p>
<p>Of course, the approach could also be extended to types of handler other than a
<a href="#id196"><span id="user-content-id197">:class:`~logging.FileHandler`</span></a> - for example, one of the rotating file handlers,
or a different type of handler altogether.</p>
<pre>.. currentmodule:: logging

</pre>
<a name="user-content-using-particular-formatting-styles-throughout-your-application"></a>
<h2><a id="user-content-using-particular-formatting-styles-throughout-your-application" class="anchor" aria-hidden="true" href="#using-particular-formatting-styles-throughout-your-application"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Using particular formatting styles throughout your application</h2>
<p>In Python 3.2, the <a href="#id198"><span id="user-content-id199">:class:`~logging.Formatter`</span></a> gained a <code>style</code> keyword
parameter which, while defaulting to <code>%</code> for backward compatibility, allowed
the specification of <code>{</code> or <code>$</code> to support the formatting approaches
supported by <a href="#id200"><span id="user-content-id201">:meth:`str.format`</span></a> and <a href="#id202"><span id="user-content-id203">:class:`string.Template`</span></a>. Note that this
governs the formatting of logging messages for final output to logs, and is
completely orthogonal to how an individual logging message is constructed.</p>
<p>Logging calls (<a href="#id204"><span id="user-content-id205">:meth:`~Logger.debug`</span></a>, <a href="#id206"><span id="user-content-id207">:meth:`~Logger.info`</span></a> etc.) only take
positional parameters for the actual logging message itself, with keyword
parameters used only for determining options for how to handle the logging call
(e.g. the <code>exc_info</code> keyword parameter to indicate that traceback information
should be logged, or the <code>extra</code> keyword parameter to indicate additional
contextual information to be added to the log). So you cannot directly make
logging calls using <a href="#id208"><span id="user-content-id209">:meth:`str.format`</span></a> or <a href="#id210"><span id="user-content-id211">:class:`string.Template`</span></a> syntax,
because internally the logging package uses %-formatting to merge the format
string and the variable arguments. There would no changing this while preserving
backward compatibility, since all logging calls which are out there in existing
code will be using %-format strings.</p>
<p>There have been suggestions to associate format styles with specific loggers,
but that approach also runs into backward compatibility problems because any
existing code could be using a given logger name and using %-formatting.</p>
<p>For logging to work interoperably between any third-party libraries and your
code, decisions about formatting need to be made at the level of the
individual logging call. This opens up a couple of ways in which alternative
formatting styles can be accommodated.</p>
<a name="user-content-using-logrecord-factories"></a>
<h3><a id="user-content-using-logrecord-factories" class="anchor" aria-hidden="true" href="#using-logrecord-factories"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Using LogRecord factories</h3>
<p>In Python 3.2, along with the <a href="#id212"><span id="user-content-id213">:class:`~logging.Formatter`</span></a> changes mentioned
above, the logging package gained the ability to allow users to set their own
<a href="#id214"><span id="user-content-id215">:class:`LogRecord`</span></a> subclasses, using the <a href="#id216"><span id="user-content-id217">:func:`setLogRecordFactory`</span></a> function.
You can use this to set your own subclass of <a href="#id218"><span id="user-content-id219">:class:`LogRecord`</span></a>, which does the
Right Thing by overriding the <a href="#id220"><span id="user-content-id221">:meth:`~LogRecord.getMessage`</span></a> method. The base
class implementation of this method is where the <code>msg % args</code> formatting
happens, and where you can substitute your alternate formatting; however, you
should be careful to support all formatting styles and allow %-formatting as
the default, to ensure interoperability with other code. Care should also be
taken to call <code>str(self.msg)</code>, just as the base implementation does.</p>
<p>Refer to the reference documentation on <a href="#id222"><span id="user-content-id223">:func:`setLogRecordFactory`</span></a> and
<a href="#id224"><span id="user-content-id225">:class:`LogRecord`</span></a> for more information.</p>
<a name="user-content-using-custom-message-objects"></a>
<h3><a id="user-content-using-custom-message-objects" class="anchor" aria-hidden="true" href="#using-custom-message-objects"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Using custom message objects</h3>
<p>There is another, perhaps simpler way that you can use {}- and $- formatting to
construct your individual log messages. You may recall (from
<a href="#id226"><span id="user-content-id227">:ref:`arbitrary-object-messages`</span></a>) that when logging you can use an arbitrary
object as a message format string, and that the logging package will call
<a href="#id228"><span id="user-content-id229">:func:`str`</span></a> on that object to get the actual format string. Consider the
following two classes:</p>
<pre>class BraceMessage(object):
    def __init__(self, fmt, *args, **kwargs):
        self.fmt = fmt
        self.args = args
        self.kwargs = kwargs

    def __str__(self):
        return self.fmt.format(*self.args, **self.kwargs)

class DollarMessage(object):
    def __init__(self, fmt, **kwargs):
        self.fmt = fmt
        self.kwargs = kwargs

    def __str__(self):
        from string import Template
        return Template(self.fmt).substitute(**self.kwargs)
</pre>
<p>Either of these can be used in place of a format string, to allow {}- or
$-formatting to be used to build the actual "message" part which appears in the
formatted log output in place of “%(message)s” or “{message}” or “$message”.
If you find it a little unwieldy to use the class names whenever you want to log
something, you can make it more palatable if you use an alias such as <code>M</code> or
<code>_</code> for the message (or perhaps <code>__</code>, if you are using <code>_</code> for
localization).</p>
<p>Examples of this approach are given below. Firstly, formatting with
<a href="#id230"><span id="user-content-id231">:meth:`str.format`</span></a>:</p>
<pre>&gt;&gt;&gt; __ = BraceMessage
&gt;&gt;&gt; print(__('Message with {0} {1}', 2, 'placeholders'))
Message with 2 placeholders
&gt;&gt;&gt; class Point: pass
...
&gt;&gt;&gt; p = Point()
&gt;&gt;&gt; p.x = 0.5
&gt;&gt;&gt; p.y = 0.5
&gt;&gt;&gt; print(__('Message with coordinates: ({point.x:.2f}, {point.y:.2f})', point=p))
Message with coordinates: (0.50, 0.50)
</pre>
<p>Secondly, formatting with <a href="#id232"><span id="user-content-id233">:class:`string.Template`</span></a>:</p>
<pre>&gt;&gt;&gt; __ = DollarMessage
&gt;&gt;&gt; print(__('Message with $num $what', num=2, what='placeholders'))
Message with 2 placeholders
&gt;&gt;&gt;
</pre>
<p>One thing to note is that you pay no significant performance penalty with this
approach: the actual formatting happens not when you make the logging call, but
when (and if) the logged message is actually about to be output to a log by a
handler. So the only slightly unusual thing which might trip you up is that the
parentheses go around the format string and the arguments, not just the format
string. That’s because the __ notation is just syntax sugar for a constructor
call to one of the <code>XXXMessage</code> classes shown above.</p>
<pre>.. currentmodule:: logging.config

</pre>
<a name="user-content-configuring-filters-with-func-dictconfig"></a>
<h2><a id="user-content-configuring-filters-with-funcdictconfig" class="anchor" aria-hidden="true" href="#configuring-filters-with-funcdictconfig"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Configuring filters with <a href="#id234"><span id="user-content-id235">:func:`dictConfig`</span></a></h2>
<p>You <em>can</em> configure filters using <a href="#id236"><span id="user-content-id237">:func:`~logging.config.dictConfig`</span></a>, though it
might not be obvious at first glance how to do it (hence this recipe). Since
<a href="#id238"><span id="user-content-id239">:class:`~logging.Filter`</span></a> is the only filter class included in the standard
library, and it is unlikely to cater to many requirements (it's only there as a
base class), you will typically need to define your own <a href="#id240"><span id="user-content-id241">:class:`~logging.Filter`</span></a>
subclass with an overridden <a href="#id242"><span id="user-content-id243">:meth:`~logging.Filter.filter`</span></a> method. To do this,
specify the <code>()</code> key in the configuration dictionary for the filter,
specifying a callable which will be used to create the filter (a class is the
most obvious, but you can provide any callable which returns a
<a href="#id244"><span id="user-content-id245">:class:`~logging.Filter`</span></a> instance). Here is a complete example:</p>
<pre>import logging
import logging.config
import sys

class MyFilter(logging.Filter):
    def __init__(self, param=None):
        self.param = param

    def filter(self, record):
        if self.param is None:
            allow = True
        else:
            allow = self.param not in record.msg
        if allow:
            record.msg = 'changed: ' + record.msg
        return allow

LOGGING = {
    'version': 1,
    'filters': {
        'myfilter': {
            '()': MyFilter,
            'param': 'noshow',
        }
    },
    'handlers': {
        'console': {
            'class': 'logging.StreamHandler',
            'filters': ['myfilter']
        }
    },
    'root': {
        'level': 'DEBUG',
        'handlers': ['console']
    },
}

if __name__ == '__main__':
    logging.config.dictConfig(LOGGING)
    logging.debug('hello')
    logging.debug('hello - noshow')
</pre>
<p>This example shows how you can pass configuration data to the callable which
constructs the instance, in the form of keyword parameters. When run, the above
script will print:</p>
<pre lang="none">changed: hello
</pre>
<p>which shows that the filter is working as configured.</p>
<p>A couple of extra points to note:</p>
<ul>
<li>If you can't refer to the callable directly in the configuration (e.g. if it
lives in a different module, and you can't import it directly where the
configuration dictionary is), you can use the form <code>ext://...</code> as described
in <a href="#id246"><span id="user-content-id247">:ref:`logging-config-dict-externalobj`</span></a>. For example, you could have used
the text <code>'ext://__main__.MyFilter'</code> instead of <code>MyFilter</code> in the above
example.</li>
<li>As well as for filters, this technique can also be used to configure custom
handlers and formatters. See <a href="#id248"><span id="user-content-id249">:ref:`logging-config-dict-userdef`</span></a> for more
information on how logging supports using user-defined objects in its
configuration, and see the other cookbook recipe <a href="#id250"><span id="user-content-id251">:ref:`custom-handlers`</span></a> above.</li>
</ul>
<a name="user-content-customized-exception-formatting"></a>
<h2><a id="user-content-customized-exception-formatting" class="anchor" aria-hidden="true" href="#customized-exception-formatting"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Customized exception formatting</h2>
<p>There might be times when you want to do customized exception formatting - for
argument's sake, let's say you want exactly one line per logged event, even
when exception information is present. You can do this with a custom formatter
class, as shown in the following example:</p>
<pre>import logging

class OneLineExceptionFormatter(logging.Formatter):
    def formatException(self, exc_info):
        """
        Format an exception so that it prints on a single line.
        """
        result = super(OneLineExceptionFormatter, self).formatException(exc_info)
        return repr(result)  # or format into one line however you want to

    def format(self, record):
        s = super(OneLineExceptionFormatter, self).format(record)
        if record.exc_text:
            s = s.replace('\n', '') + '|'
        return s

def configure_logging():
    fh = logging.FileHandler('output.txt', 'w')
    f = OneLineExceptionFormatter('%(asctime)s|%(levelname)s|%(message)s|',
                                  '%d/%m/%Y %H:%M:%S')
    fh.setFormatter(f)
    root = logging.getLogger()
    root.setLevel(logging.DEBUG)
    root.addHandler(fh)

def main():
    configure_logging()
    logging.info('Sample message')
    try:
        x = 1 / 0
    except ZeroDivisionError as e:
        logging.exception('ZeroDivisionError: %s', e)

if __name__ == '__main__':
    main()
</pre>
<p>When run, this produces a file with exactly two lines:</p>
<pre lang="none">28/01/2015 07:21:23|INFO|Sample message|
28/01/2015 07:21:23|ERROR|ZeroDivisionError: integer division or modulo by zero|'Traceback (most recent call last):\n  File "logtest7.py", line 30, in main\n    x = 1 / 0\nZeroDivisionError: integer division or modulo by zero'|
</pre>
<p>While the above treatment is simplistic, it points the way to how exception
information can be formatted to your liking. The <a href="#id252"><span id="user-content-id253">:mod:`traceback`</span></a> module may be
helpful for more specialized needs.</p>
<a name="user-content-speaking-logging-messages"></a>
<h2><a id="user-content-speaking-logging-messages" class="anchor" aria-hidden="true" href="#speaking-logging-messages"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Speaking logging messages</h2>
<p>There might be situations when it is desirable to have logging messages rendered
in an audible rather than a visible format. This is easy to do if you have
text-to-speech (TTS) functionality available in your system, even if it doesn't have
a Python binding. Most TTS systems have a command line program you can run, and
this can be invoked from a handler using <a href="#id254"><span id="user-content-id255">:mod:`subprocess`</span></a>. It's assumed here
that TTS command line programs won't expect to interact with users or take a
long time to complete, and that the frequency of logged messages will be not so
high as to swamp the user with messages, and that it's acceptable to have the
messages spoken one at a time rather than concurrently, The example implementation
below waits for one message to be spoken before the next is processed, and this
might cause other handlers to be kept waiting. Here is a short example showing
the approach, which assumes that the <code>espeak</code> TTS package is available:</p>
<pre>import logging
import subprocess
import sys

class TTSHandler(logging.Handler):
    def emit(self, record):
        msg = self.format(record)
        # Speak slowly in a female English voice
        cmd = ['espeak', '-s150', '-ven+f3', msg]
        p = subprocess.Popen(cmd, stdout=subprocess.PIPE,
                             stderr=subprocess.STDOUT)
        # wait for the program to finish
        p.communicate()

def configure_logging():
    h = TTSHandler()
    root = logging.getLogger()
    root.addHandler(h)
    # the default formatter just returns the message
    root.setLevel(logging.DEBUG)

def main():
    logging.info('Hello')
    logging.debug('Goodbye')

if __name__ == '__main__':
    configure_logging()
    sys.exit(main())
</pre>
<p>When run, this script should say "Hello" and then "Goodbye" in a female voice.</p>
<p>The above approach can, of course, be adapted to other TTS systems and even
other systems altogether which can process messages via external programs run
from a command line.</p>
<a name="user-content-buffering-logging-messages-and-outputting-them-conditionally"></a>
<h2><a id="user-content-buffering-logging-messages-and-outputting-them-conditionally" class="anchor" aria-hidden="true" href="#buffering-logging-messages-and-outputting-them-conditionally"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Buffering logging messages and outputting them conditionally</h2>
<p>There might be situations where you want to log messages in a temporary area
and only output them if a certain condition occurs. For example, you may want to
start logging debug events in a function, and if the function completes without
errors, you don't want to clutter the log with the collected debug information,
but if there is an error, you want all the debug information to be output as well
as the error.</p>
<p>Here is an example which shows how you could do this using a decorator for your
functions where you want logging to behave this way. It makes use of the
<a href="#id256"><span id="user-content-id257">:class:`logging.handlers.MemoryHandler`</span></a>, which allows buffering of logged events
until some condition occurs, at which point the buffered events are <code>flushed</code>
- passed to another handler (the <code>target</code> handler) for processing. By default,
the <code>MemoryHandler</code> flushed when its buffer gets filled up or an event whose
level is greater than or equal to a specified threshold is seen. You can use this
recipe with a more specialised subclass of <code>MemoryHandler</code> if you want custom
flushing behavior.</p>
<p>The example script has a simple function, <code>foo</code>, which just cycles through
all the logging levels, writing to <code>sys.stderr</code> to say what level it's about
to log at, and then actually logging a message at that level. You can pass a
parameter to <code>foo</code> which, if true, will log at ERROR and CRITICAL levels -
otherwise, it only logs at DEBUG, INFO and WARNING levels.</p>
<p>The script just arranges to decorate <code>foo</code> with a decorator which will do the
conditional logging that's required. The decorator takes a logger as a parameter
and attaches a memory handler for the duration of the call to the decorated
function. The decorator can be additionally parameterised using a target handler,
a level at which flushing should occur, and a capacity for the buffer. These
default to a <a href="#id258"><span id="user-content-id259">:class:`~logging.StreamHandler`</span></a> which writes to <code>sys.stderr</code>,
<code>logging.ERROR</code> and <code>100</code> respectively.</p>
<p>Here's the script:</p>
<pre>import logging
from logging.handlers import MemoryHandler
import sys

logger = logging.getLogger(__name__)
logger.addHandler(logging.NullHandler())

def log_if_errors(logger, target_handler=None, flush_level=None, capacity=None):
    if target_handler is None:
        target_handler = logging.StreamHandler()
    if flush_level is None:
        flush_level = logging.ERROR
    if capacity is None:
        capacity = 100
    handler = MemoryHandler(capacity, flushLevel=flush_level, target=target_handler)

    def decorator(fn):
        def wrapper(*args, **kwargs):
            logger.addHandler(handler)
            try:
                return fn(*args, **kwargs)
            except Exception:
                logger.exception('call failed')
                raise
            finally:
                super(MemoryHandler, handler).flush()
                logger.removeHandler(handler)
        return wrapper

    return decorator

def write_line(s):
    sys.stderr.write('%s\n' % s)

def foo(fail=False):
    write_line('about to log at DEBUG ...')
    logger.debug('Actually logged at DEBUG')
    write_line('about to log at INFO ...')
    logger.info('Actually logged at INFO')
    write_line('about to log at WARNING ...')
    logger.warning('Actually logged at WARNING')
    if fail:
        write_line('about to log at ERROR ...')
        logger.error('Actually logged at ERROR')
        write_line('about to log at CRITICAL ...')
        logger.critical('Actually logged at CRITICAL')
    return fail

decorated_foo = log_if_errors(logger)(foo)

if __name__ == '__main__':
    logger.setLevel(logging.DEBUG)
    write_line('Calling undecorated foo with False')
    assert not foo(False)
    write_line('Calling undecorated foo with True')
    assert foo(True)
    write_line('Calling decorated foo with False')
    assert not decorated_foo(False)
    write_line('Calling decorated foo with True')
    assert decorated_foo(True)
</pre>
<p>When this script is run, the following output should be observed:</p>
<pre lang="none">Calling undecorated foo with False
about to log at DEBUG ...
about to log at INFO ...
about to log at WARNING ...
Calling undecorated foo with True
about to log at DEBUG ...
about to log at INFO ...
about to log at WARNING ...
about to log at ERROR ...
about to log at CRITICAL ...
Calling decorated foo with False
about to log at DEBUG ...
about to log at INFO ...
about to log at WARNING ...
Calling decorated foo with True
about to log at DEBUG ...
about to log at INFO ...
about to log at WARNING ...
about to log at ERROR ...
Actually logged at DEBUG
Actually logged at INFO
Actually logged at WARNING
Actually logged at ERROR
about to log at CRITICAL ...
Actually logged at CRITICAL
</pre>
<p>As you can see, actual logging output only occurs when an event is logged whose
severity is ERROR or greater, but in that case, any previous events at lower
severities are also logged.</p>
<p>You can of course use the conventional means of decoration:</p>
<pre>@log_if_errors(logger)
def foo(fail=False):
    ...
</pre>
<a name="user-content-formatting-times-using-utc-gmt-via-configuration"></a>
<h2><a id="user-content-formatting-times-using-utc-gmt-via-configuration" class="anchor" aria-hidden="true" href="#formatting-times-using-utc-gmt-via-configuration"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Formatting times using UTC (GMT) via configuration</h2>
<p>Sometimes you want to format times using UTC, which can be done using a class
such as UTCFormatter, shown below:</p>
<pre>import logging
import time

class UTCFormatter(logging.Formatter):
    converter = time.gmtime
</pre>
<p>and you can then use the <code>UTCFormatter</code> in your code instead of
<a href="#id260"><span id="user-content-id261">:class:`~logging.Formatter`</span></a>. If you want to do that via configuration, you can
use the <a href="#id262"><span id="user-content-id263">:func:`~logging.config.dictConfig`</span></a> API with an approach illustrated by
the following complete example:</p>
<pre>import logging
import logging.config
import time

class UTCFormatter(logging.Formatter):
    converter = time.gmtime

LOGGING = {
    'version': 1,
    'disable_existing_loggers': False,
    'formatters': {
        'utc': {
            '()': UTCFormatter,
            'format': '%(asctime)s %(message)s',
        },
        'local': {
            'format': '%(asctime)s %(message)s',
        }
    },
    'handlers': {
        'console1': {
            'class': 'logging.StreamHandler',
            'formatter': 'utc',
        },
        'console2': {
            'class': 'logging.StreamHandler',
            'formatter': 'local',
        },
    },
    'root': {
        'handlers': ['console1', 'console2'],
   }
}

if __name__ == '__main__':
    logging.config.dictConfig(LOGGING)
    logging.warning('The local time is %s', time.asctime())
</pre>
<p>When this script is run, it should print something like:</p>
<pre lang="none">2015-10-17 12:53:29,501 The local time is Sat Oct 17 13:53:29 2015
2015-10-17 13:53:29,501 The local time is Sat Oct 17 13:53:29 2015
</pre>
<p>showing how the time is formatted both as local time and UTC, one for each
handler.</p>
<a name="user-content-using-a-context-manager-for-selective-logging"></a>
<h2><a id="user-content-using-a-context-manager-for-selective-logging" class="anchor" aria-hidden="true" href="#using-a-context-manager-for-selective-logging"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Using a context manager for selective logging</h2>
<p>There are times when it would be useful to temporarily change the logging
configuration and revert it back after doing something. For this, a context
manager is the most obvious way of saving and restoring the logging context.
Here is a simple example of such a context manager, which allows you to
optionally change the logging level and add a logging handler purely in the
scope of the context manager:</p>
<pre>import logging
import sys

class LoggingContext(object):
    def __init__(self, logger, level=None, handler=None, close=True):
        self.logger = logger
        self.level = level
        self.handler = handler
        self.close = close

    def __enter__(self):
        if self.level is not None:
            self.old_level = self.logger.level
            self.logger.setLevel(self.level)
        if self.handler:
            self.logger.addHandler(self.handler)

    def __exit__(self, et, ev, tb):
        if self.level is not None:
            self.logger.setLevel(self.old_level)
        if self.handler:
            self.logger.removeHandler(self.handler)
        if self.handler and self.close:
            self.handler.close()
        # implicit return of None =&gt; don't swallow exceptions
</pre>
<p>If you specify a level value, the logger's level is set to that value in the
scope of the with block covered by the context manager. If you specify a
handler, it is added to the logger on entry to the block and removed on exit
from the block. You can also ask the manager to close the handler for you on
block exit - you could do this if you don't need the handler any more.</p>
<p>To illustrate how it works, we can add the following block of code to the
above:</p>
<pre>if __name__ == '__main__':
    logger = logging.getLogger('foo')
    logger.addHandler(logging.StreamHandler())
    logger.setLevel(logging.INFO)
    logger.info('1. This should appear just once on stderr.')
    logger.debug('2. This should not appear.')
    with LoggingContext(logger, level=logging.DEBUG):
        logger.debug('3. This should appear once on stderr.')
    logger.debug('4. This should not appear.')
    h = logging.StreamHandler(sys.stdout)
    with LoggingContext(logger, level=logging.DEBUG, handler=h, close=True):
        logger.debug('5. This should appear twice - once on stderr and once on stdout.')
    logger.info('6. This should appear just once on stderr.')
    logger.debug('7. This should not appear.')
</pre>
<p>We initially set the logger's level to <code>INFO</code>, so message #1 appears and
message #2 doesn't. We then change the level to <code>DEBUG</code> temporarily in the
following <code>with</code> block, and so message #3 appears. After the block exits, the
logger's level is restored to <code>INFO</code> and so message #4 doesn't appear. In the
next <code>with</code> block, we set the level to <code>DEBUG</code> again but also add a handler
writing to <code>sys.stdout</code>. Thus, message #5 appears twice on the console (once
via <code>stderr</code> and once via <code>stdout</code>). After the <code>with</code> statement's
completion, the status is as it was before so message #6 appears (like message
#1) whereas message #7 doesn't (just like message #2).</p>
<p>If we run the resulting script, the result is as follows:</p>
<pre lang="shell-session">$ python logctx.py
1. This should appear just once on stderr.
3. This should appear once on stderr.
5. This should appear twice - once on stderr and once on stdout.
5. This should appear twice - once on stderr and once on stdout.
6. This should appear just once on stderr.
</pre>
<p>If we run it again, but pipe <code>stderr</code> to <code>/dev/null</code>, we see the following,
which is the only message written to <code>stdout</code>:</p>
<pre lang="shell-session">$ python logctx.py 2&gt;/dev/null
5. This should appear twice - once on stderr and once on stdout.
</pre>
<p>Once again, but piping <code>stdout</code> to <code>/dev/null</code>, we get:</p>
<pre lang="shell-session">$ python logctx.py &gt;/dev/null
1. This should appear just once on stderr.
3. This should appear once on stderr.
5. This should appear twice - once on stderr and once on stdout.
6. This should appear just once on stderr.
</pre>
<p>In this case, the message #5 printed to <code>stdout</code> doesn't appear, as expected.</p>
<p>Of course, the approach described here can be generalised, for example to attach
logging filters temporarily. Note that the above code works in Python 2 as well
as Python 3.</p>
<a name="user-content-a-cli-application-starter-template"></a>
<h2><a id="user-content-a-cli-application-starter-template" class="anchor" aria-hidden="true" href="#a-cli-application-starter-template"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>A CLI application starter template</h2>
<p>Here's an example which shows how you can:</p>
<ul>
<li>Use a logging level based on command-line arguments</li>
<li>Dispatch to multiple subcommands in separate files, all logging at the same
level in a consistent way</li>
<li>Make use of simple, minimal configuration</li>
</ul>
<p>Suppose we have a command-line application whose job is to stop, start or
restart some services. This could be organised for the purposes of illustration
as a file <code>app.py</code> that is the main script for the application, with individual
commands implemented in <code>start.py</code>, <code>stop.py</code> and <code>restart.py</code>. Suppose
further that we want to control the verbosity of the application via a
command-line argument, defaulting to <code>logging.INFO</code>. Here's one way that
<code>app.py</code> could be written:</p>
<pre>import argparse
import importlib
import logging
import os
import sys

def main(args=None):
    scriptname = os.path.basename(__file__)
    parser = argparse.ArgumentParser(scriptname)
    levels = ('DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL')
    parser.add_argument('--log-level', default='INFO', choices=levels)
    subparsers = parser.add_subparsers(dest='command',
                                       help='Available commands:')
    start_cmd = subparsers.add_parser('start', help='Start a service')
    start_cmd.add_argument('name', metavar='NAME',
                           help='Name of service to start')
    stop_cmd = subparsers.add_parser('stop',
                                     help='Stop one or more services')
    stop_cmd.add_argument('names', metavar='NAME', nargs='+',
                          help='Name of service to stop')
    restart_cmd = subparsers.add_parser('restart',
                                        help='Restart one or more services')
    restart_cmd.add_argument('names', metavar='NAME', nargs='+',
                             help='Name of service to restart')
    options = parser.parse_args()
    # the code to dispatch commands could all be in this file. For the purposes
    # of illustration only, we implement each command in a separate module.
    try:
        mod = importlib.import_module(options.command)
        cmd = getattr(mod, 'command')
    except (ImportError, AttributeError):
        print('Unable to find the code for command \'%s\'' % options.command)
        return 1
    # Could get fancy here and load configuration from file or dictionary
    logging.basicConfig(level=options.log_level,
                        format='%(levelname)s %(name)s %(message)s')
    cmd(options)

if __name__ == '__main__':
    sys.exit(main())
</pre>
<p>And the <code>start</code>, <code>stop</code> and <code>restart</code> commands can be implemented in
separate modules, like so for starting:</p>
<pre># start.py
import logging

logger = logging.getLogger(__name__)

def command(options):
    logger.debug('About to start %s', options.name)
    # actually do the command processing here ...
    logger.info('Started the \'%s\' service.', options.name)
</pre>
<p>and thus for stopping:</p>
<pre># stop.py
import logging

logger = logging.getLogger(__name__)

def command(options):
    n = len(options.names)
    if n == 1:
        plural = ''
        services = '\'%s\'' % options.names[0]
    else:
        plural = 's'
        services = ', '.join('\'%s\'' % name for name in options.names)
        i = services.rfind(', ')
        services = services[:i] + ' and ' + services[i + 2:]
    logger.debug('About to stop %s', services)
    # actually do the command processing here ...
    logger.info('Stopped the %s service%s.', services, plural)
</pre>
<p>and similarly for restarting:</p>
<pre># restart.py
import logging

logger = logging.getLogger(__name__)

def command(options):
    n = len(options.names)
    if n == 1:
        plural = ''
        services = '\'%s\'' % options.names[0]
    else:
        plural = 's'
        services = ', '.join('\'%s\'' % name for name in options.names)
        i = services.rfind(', ')
        services = services[:i] + ' and ' + services[i + 2:]
    logger.debug('About to restart %s', services)
    # actually do the command processing here ...
    logger.info('Restarted the %s service%s.', services, plural)
</pre>
<p>If we run this application with the default log level, we get output like this:</p>
<pre lang="shell-session">$ python app.py start foo
INFO start Started the 'foo' service.

$ python app.py stop foo bar
INFO stop Stopped the 'foo' and 'bar' services.

$ python app.py restart foo bar baz
INFO restart Restarted the 'foo', 'bar' and 'baz' services.
</pre>
<p>The first word is the logging level, and the second word is the module or
package name of the place where the event was logged.</p>
<p>If we change the logging level, then we can change the information sent to the
log. For example, if we want more information:</p>
<pre lang="shell-session">$ python app.py --log-level DEBUG start foo
DEBUG start About to start foo
INFO start Started the 'foo' service.

$ python app.py --log-level DEBUG stop foo bar
DEBUG stop About to stop 'foo' and 'bar'
INFO stop Stopped the 'foo' and 'bar' services.

$ python app.py --log-level DEBUG restart foo bar baz
DEBUG restart About to restart 'foo', 'bar' and 'baz'
INFO restart Restarted the 'foo', 'bar' and 'baz' services.
</pre>
<p>And if we want less:</p>
<pre lang="shell-session">$ python app.py --log-level WARNING start foo
$ python app.py --log-level WARNING stop foo bar
$ python app.py --log-level WARNING restart foo bar baz
</pre>
<p>In this case, the commands don't print anything to the console, since nothing
at <code>WARNING</code> level or above is logged by them.</p>

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
      <li class="mr-3">&copy; 2019 <span title="0.32560s from unicorn-845bd54489-9k8bf">GitHub</span>, Inc.</li>
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

