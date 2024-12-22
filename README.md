# Intro

As Discogs buyers, we tend to prefer sellers who have multiple items from our wantlist. This allows us to order several records while minimizing shipping costs.

# Problem
The Discogs engine matches a seller’s inventory to our wantlist strictly by release. If we forget to include all versions of a specific master release (such as different pressings or editions of the same album) in our wantlist, they won’t be matched with the seller’s inventory. For example, if an album has two pressings, X and Y, and you only have X on your wantlist, a seller offering Y won’t be suggested to you, even though it’s the same band and album.
# Solution
The code enhances matching by using the API to fetch master IDs from your wantlist, retrieving the seller’s inventory, gathering all release versions of matched master releases, and cross-referencing them to identify matches between the wantlist and the seller’s inventory.
## Example
With Discogs Wantlist Search

<img width="1116" alt="image" src="https://github.com/user-attachments/assets/47924828-3f0a-4cad-9b06-1118f9537b1a" />

With [Enhanced Wantlist Search]([url](https://github.com/OpAlliance/discogs_wantlist_inventory_matcher/blob/main/wantlist_vs_seller_matcher.ipynb))

<img width="648" alt="image" src="https://github.com/user-attachments/assets/bf1bbaf2-af0b-4b4f-9223-eb212d76107c" />
<img width="1281" alt="image" src="https://github.com/user-attachments/assets/ca42db94-3aa2-409e-9499-7fb81c2af6ec" />

<img width="1238" alt="image" src="https://github.com/user-attachments/assets/210e66fe-7acf-403b-9371-db54dbbd9837" /> 

