# Git Recursive Submodule

This project contains recursive Git submodules for validating sonar-text.
The project structure:

```
<repo root>
|- submodule sonar-iac
   |- submodule ibm-tf-training (recursive)
   |- submodule terraform-aws-secure-baseline (recursive)
   |- submodule terragoat (recursive)
   |- ... (more)
|- submodule ibm-tf-training (in root)
|- submodule terraform-aws-secure-baseline (in root)
|- submodule terragoat (in root)
|- example-secrets.properties (a file containing some secrets)
```

Initialize the submodules:

```
git submodule update --init --recursive
```

