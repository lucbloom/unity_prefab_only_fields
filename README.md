# PrefabOnly and InstanceOnly properties
Include or exclude class field in the Inspector when in Prefab Mode or outside, viewing an Instance of that Prefab.

-  [SerializeField, PrefabOnly] Material SpriteMat;
-  [SerializeField, PrefabOnly] Sprite ProgressBarFill;
-  [SerializeField, PrefabOnly] Sprite ProgressBarCap;
-  [SerializeField, PrefabOnly] string LoadingTerm;

-  [SerializeField, InstanceOnly] ProgressBarManager Manager;
-  [SerializeField, InstanceOnly] Transform IntanceParent;
-  [SerializeField, InstanceOnly] string CaptionTerm;

This way, your inspector isn't cluttered with stuff you don't want to (or shouldn't) see.
Think of PrefabOnly like "private" for the Prefab. 
Think of InstanceOnly like "public" for the Prefab's user. But hidden when inside the prefab so you're not confronted with [None] references or default values for fields that should be filled in per instance.
