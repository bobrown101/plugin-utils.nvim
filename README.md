# file-utils.nvim
Common lua functions plugins might want to reuse instead of rewrite


## Install
```lua

    use({"bobrown101/plugin-utils.nvim"})

    -- If there is another plugin that depends on plugin-utils, you can denote that with packer like so
    use({
        "other plugin that depends on it",
        requires = {"bobrown101/plugin-utils.nvim"},
        config = function() require("other plugin that depends on it").setup({}) end
    })

```

## Use
```lua
local buffer_find_root_dir =
    require('bobrown101.plugin-utils').buffer_find_root_dir;
```
