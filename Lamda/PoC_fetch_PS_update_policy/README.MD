# PoC fetch PS and update policy description

- Lambda is triggered by Amazon EventBridge which monitors changes in Parameter Store.
- When change occurs, Lamda fetches AWS account ID from the Parameter Store and updates principals in the local bucket_policy.json.
- Policy is updated and than applied as a bucket policy on specified bucket.