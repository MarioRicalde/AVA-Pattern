    /stylesheets/
      vendor/
        survival-kit/                 # Has custom dir and partials.
          ...
        jquery-ui/                    # Has custom dir and partials.
          ...

      app/                          # Directory name reflecting the "master" file. (mobile, iphone, ie, w/e)
        _forums.scss                # General idea of the dir, includes partials inside current_dir.
        _posts.scss                 # General idea of the dir, includes partials inside current_dir.
        _comments.scss              # General idea of the dir, includes partials inside current_dir.
        forums/                      
          _thread.scss                
          _thread-listing.scss        
        posts/                        
          _posts-listing.scss         
        comments/                     
          _comment-listing.scss       
        shared/                       
          _headers.scss               
          _footers.scss               
          _content.scss               
          _sidebar.scss               
      mobile/             
        _forums.scss                # General idea of the dir, includes partials inside current_dir.
        _posts.scss                 # General idea of the dir, includes partials inside current_dir.
        _comments.scss              # General idea of the dir, includes partials inside current_dir.            
        forums/                       
          _thread.scss                
          _thread-listing.scss        
        posts/                        
          _post-listing.scss          
        comments/                     
          _comment-listing.scss       
        shared/                      
          _headers.scss              
          _footers.scss              
          _content.scss              
          _sidebar.scss              
                             
      mobile.scss                     # Includes everything under mobile/
      app.scss                        # Includes everything under app/
                             
    /images/                         
      vendor/                         # Images related to a vendor library.
        survival-kit/                
          ...                        
        jquery-ui/                   
          ...                        
      app/                            # Images related to the 'app' version of the site.
        bg-header.png                
        bg-content.png               
        sp-user-interface.png        
      mobile/                         # Images related to the 'mobile' version of the site.
        bg-header.png                
        bg-content.png               
        sp-user-interface.png        
                             
    /javascripts/                    
      tests/                          # Tests.
        ..                           
      vendor/                        
        survival-kit/                
          ..                         
        jquery-ui/                   
          ..                         
      app/                            # JS Files for 'mobile'
        forums.coffee                 # Rails way, one file per controller.
        posts.coffee                 
        comments.coffee              
        shared/                      
          functionality-1.coffee     
          functionality-2.coffee     
      mobile/                         # JS Files for 'mobile'
        forums.coffee
        posts.coffee
        comments.coffee
        shared/
          functionality-1.coffee
          functionality-2.coffee
      mobile.js                       # Includes all mobile/ js files
      app.js                          # Include all app/ js files