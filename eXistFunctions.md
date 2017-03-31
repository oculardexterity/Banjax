eXist Operations


GET -- 
/doc/text          - as xml node
/doc/metadata      -- as xml nodelist

/collection/             -- as xml nodelist

/collection///           -- as some custom format (graph? whatever)


POST (create new) --
/item               -- xml template file


PATCH (update) --
/doc/text           -- xupdate object: overwrite text
/doc/metadata       -- overwrite each metadata field
