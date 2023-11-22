# pythoneda-sandbox/python-dep

Definition of <https://github.com/pythoneda-sandbox/python-dep>.

## How to declare it in your flake

Check the latest tag of this repository and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-sandbox-python-dep = {
      [optional follows]
      url =
        "github:pythoneda-sandbox-def/python-dep/[version]";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [nixpkgs](https://github.com/nixos/nixpkgs "nixpkgs") and [flake-utils](https://github.com/numtide/flake-utils "flake-utils").

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-sandbox-python-dep-python38` 
- `#packages.[system].pythoneda-sandbox-python-dep-python39` 
- `#packages.[system].pythoneda-sandbox-python-dep-python310` 
- `#packages.[system].pythoneda-sandbox-python-dep-python311` 
