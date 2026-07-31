---
id: dc96d568b258
type: remark
lean:
  - SpherePacking
formalized: true
---

# Remark — SpherePacking

## Statement

> [!remark] SpherePacking
> Note that a [[spherepackingballs|sphere packing]] is uniquely defined from a given set of centres (which, in order to be a valid set of centres, must admit a corresponding [[spherepackingballs|separation radius]]). Therefore, as a conscious choice during the formalisation process, we will define everything that depends on sphere packings in terms of `SpherePacking`, a `structure` that bundles all the identifying information of a packing, but not the actual balls themselves. For the purposes of this blueprint, however, we will refrain from making this distinction.
