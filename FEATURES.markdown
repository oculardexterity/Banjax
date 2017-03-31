# Larynx/Banjax (??) Plan

## Front End Modules
    - Modifiable template for plug-in components
        - Generic page structure

    - Images Upload Form
        @ Invokes creation of new object
    - Metadata Entry Form
        @ Blank or half-complete form containing object metadata (generated from form-builder)
        @ Does this return form and ajax in data or build all on fly? -- advantage of latter: page and assets can be returned directly from webserver static files
    - Transcriber Interface
        @ Generic interface generated from configs
        @ Ajax call to server for XML <text> element
    - Editor Interface
        @ as TInt
    - Display Interface
        @ Ajax call to eXist for data
    - Admin Interface
        - Normalised list managers
        - Users manager

## Back End Config Jobs
    - Metadata Form Generator
    - eXist data bindings setup
    - Deploy XQueries to eXist
        - Enable versioning module?
    - Push static files to 
    - Plug-in API for modules (uploader?)

## Data Layer
    - eXist Wrapper, API
        - XQueries for database read/write && mapped Python requests
    - Data validation
            - XML Schema updater (validates names etc.)
    - RevisionDesc Manager and messaging API

## Back End Functionality
    - Image Upload Handler
        - 
        - ImageMagick Async Task
        - Object Creation task
    - Router/Controller
        - Image Upload
        - Metadata
            - Persons normalisation request
            - Places normalisation request
            - Orgs normalisation request
                @ Object-lock manager
        - Transcription
            - Get request
            - Patch request
                @ Object-lock manager
        - Editor
                @ Object-lock manager
        - Display
        - Oxygen WEBDAV (direct to exist?)
        - Admin
            - Versioning control
            - User management
            - Force-unlocking 
            - Periodic Backups
            - File dumps
            - XML-config update interface (possibly triggering jobs?)
    - User log-in (Mongo/Postgres)
    - File locks



