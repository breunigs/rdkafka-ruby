# 0.4.2
* Delivery callback for producer
* Document list param of commit method
* Use default Homebrew openssl location if present
* Consumer lag handles empty topics
* End iteration in consumer when it is closed
* Add suport for storing message offsets
* Add missing runtime dependency to rake

# 0.4.1
* Bump librdkafka to 0.11.6

# 0.4.0
* Improvements in librdkafka archive download
* Add global statistics callback
* Use Time for timestamps, potentially breaking change if you
  rely on the previous behavior where it returns an integer with
  the number of milliseconds.
* Bump librdkafka to 0.11.5
* Implement TopicPartitionList in Ruby so we don't have to keep
  track of native objects.
* Support committing a topic partition list
* Add consumer assignment method

# 0.3.5
* Fix crash when not waiting for delivery handles
* Run specs on Ruby 2.5

# 0.3.4
* Bump librdkafka to 0.11.3

# 0.3.3
* Fix bug that prevent display of `RdkafkaError` message

# 0.3.2
* `add_topic` now supports using a partition count
* Add way to make errors clearer with an extra message
* Show topics in subscribe error message
* Show partition and topic in query watermark offsets error message

# 0.3.1
* Bump librdkafka to 0.11.1
* Officially support ranges in `add_topic` for topic partition list.
* Add consumer lag calculator

# 0.3.0
* Move both add topic methods to one `add_topic` in `TopicPartitionList`
* Add committed offsets to consumer
* Add query watermark offset to consumer

# 0.2.0
* Some refactoring and add inline documentation

# 0.1.x
* Initial working version including producing and consuming
