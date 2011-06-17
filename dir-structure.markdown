    /stylesheets/
      vendor/
        survival-kit/               # Has custom dir and partials.
          ...
        jquery-ui/                  # Has custom dir and partials.
          ...

      app/                          # Type
        _forums.scss                # Include files, define resource variables and global classes (for @extension)
        _posts.scss                 # Include files, define resource variables and global classes (for @extension)
        _comments.scss              # Include files, define resource variables and global classes (for @extension)
        forums/                      
          _index.scss               
          _show.scss                
          _new.scss                 
          _edit.scss                
        posts/                      
          _index.scss               
          _show.scss                
          _new.scss                 
          _edit.scss                
        comments/                   
          _index.scss               
          _show.scss                
          _new.scss                 
          _edit.scss                
        layouts/                     # DISCUSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSS
          _application.scss          # Default rails name.
          _forums.scss
        shared/                       
          _headers.scss               
          _footers.scss               
          _contents.scss               
      mobile/                        # Type
        _forums.scss                 # Include files, define resource variables and global classes (for @extension)
        _posts.scss                  # Include files, define resource variables and global classes (for @extension)
        _comments.scss               # Include files, define resource variables and global classes (for @extension)          
        forums/                      
          _index.scss               
          _show.scss                  
          _new.scss                   
          _edit.scss                  
        posts/                      
          _index.scss               
          _show.scss                  
          _new.scss                   
          _edit.scss                  
        comments/                   
          _index.scss               
          _show.scss                  
          _new.scss                   
          _edit.scss                
        shared/                      
          _headers.scss              
          _footers.scss              
          _contents.scss              
                                  
      mobile.scss                     # Include files, define resource variables and global classes (for @extension)
      app.scss                        # Include files, define resource variables and global classes (for @extension)
                         
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