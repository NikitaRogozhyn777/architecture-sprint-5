1. Лог Rasa

```bash
2025-06-03 08:53:24 DEBUG    rasa.cli.utils  - Parameter 'credentials' not set. Using default location 'credentials.yml' instead.
SANIC_VERSION = LooseVersion(sanic_version)
2025-06-03 08:53:28 DEBUG    h5py._conv  - Creating converter from 7 to 5
2025-06-03 08:53:28 DEBUG    h5py._conv  - Creating converter from 5 to 7
2025-06-03 08:53:28 DEBUG    h5py._conv  - Creating converter from 7 to 5
2025-06-03 08:53:28 DEBUG    h5py._conv  - Creating converter from 5 to 7
2025-06-03 08:53:31 DEBUG    rasa.core.utils  - Available web server routes:
/conversations/<conversation_id:path>/messages     POST                           add_message
/conversations/<conversation_id:path>/tracker/events POST                           append_events
/webhooks/rasa                                     GET                            custom_webhook_RasaChatInput.health
/webhooks/rasa/webhook                             POST                           custom_webhook_RasaChatInput.receive
/webhooks/rest                                     GET                            custom_webhook_RestInput.health
/webhooks/rest/webhook                             POST                           custom_webhook_RestInput.receive
/model/test/intents                                POST                           evaluate_intents
/model/test/stories                                POST                           evaluate_stories
/conversations/<conversation_id:path>/execute      POST                           execute_action
/domain                                            GET                            get_domain
/                                                  GET                            hello
/model                                             PUT                            load_model
/model/parse                                       POST                           parse
/conversations/<conversation_id:path>/predict      POST                           predict
/conversations/<conversation_id:path>/tracker/events PUT                            replace_events
/conversations/<conversation_id:path>/story        GET                            retrieve_story
/conversations/<conversation_id:path>/tracker      GET                            retrieve_tracker
/status                                            GET                            status
/model/predict                                     POST                           tracker_predict
/model/train                                       POST                           train
/conversations/<conversation_id:path>/trigger_intent POST                           trigger_intent
/model                                             DELETE                         unload_model
/version                                           GET                            version
2025-06-03 08:53:31 INFO     root  - Starting Rasa server on http://0.0.0.0:5005
2025-06-03 08:53:31 DEBUG    rasa.core.utils  - Using the default number of Sanic workers (1).
2025-06-03 08:53:32 DEBUG    rasa.telemetry  - Skipping telemetry reporting: no license hash found.
2025-06-03 08:53:32 DEBUG    rasa.core.tracker_store  - Connected to InMemoryTrackerStore.
2025-06-03 08:53:32 DEBUG    rasa.core.lock_store  - Connected to lock store 'InMemoryLockStore'.
2025-06-03 08:53:32 DEBUG    rasa.core.nlg.generator  - Instantiated NLG to 'TemplatedNaturalLanguageGenerator'.
2025-06-03 08:53:32 INFO     rasa.core.processor  - Loading model models/20250603-085135-grim-roundel.tar.gz...
2025-06-03 08:53:32 DEBUG    rasa.engine.storage.local_model_storage  - Extracted model to '/var/folders/mn/468p6dp91qb8p_yc3wtlxkv40000gp/T/tmpx1f6n0qu'.
2025-06-03 08:53:32 DEBUG    rasa.engine.graph  - Node 'nlu_message_converter' loading 'NLUMessageConverter.load' and kwargs: '{}'.
2025-06-03 08:53:32 DEBUG    rasa.engine.graph  - Node 'run_WhitespaceTokenizer0' loading 'WhitespaceTokenizer.load' and kwargs: '{}'.
2025-06-03 08:53:32 DEBUG    rasa.engine.graph  - Node 'run_RegexFeaturizer1' loading 'RegexFeaturizer.load' and kwargs: '{}'.
2025-06-03 08:53:32 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_RegexFeaturizer1' was requested for reading.
2025-06-03 08:53:32 DEBUG    rasa.engine.graph  - Node 'run_LexicalSyntacticFeaturizer2' loading 'LexicalSyntacticFeaturizer.load' and kwargs: '{}'.
2025-06-03 08:53:32 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_LexicalSyntacticFeaturizer2' was requested for reading.
2025-06-03 08:53:32 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer3' loading 'CountVectorsFeaturizer.load' and kwargs: '{}'.
2025-06-03 08:53:32 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_CountVectorsFeaturizer3' was requested for reading.
2025-06-03 08:53:32 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer4' loading 'CountVectorsFeaturizer.load' and kwargs: '{}'.
2025-06-03 08:53:32 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_CountVectorsFeaturizer4' was requested for reading.
2025-06-03 08:53:32 DEBUG    rasa.engine.graph  - Node 'run_DIETClassifier5' loading 'DIETClassifier.load' and kwargs: '{}'.
2025-06-03 08:53:32 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_DIETClassifier5' was requested for reading.
2025-06-03 08:53:32 DEBUG    rasa.utils.tensorflow.models  - Loading the model from /var/folders/mn/468p6dp91qb8p_yc3wtlxkv40000gp/T/tmpkcqdo7o0/train_DIETClassifier5/DIETClassifier.tf_model with finetune_mode=False...
2025-06-03 08:53:32 DEBUG    rasa.nlu.classifiers.diet_classifier  - You specified 'DIET' to train entities, but no entities are present in the training data. Skipping training of entities.
2025-06-03 08:53:32 DEBUG    rasa.nlu.classifiers.diet_classifier  - Following metrics will be logged during training:
2025-06-03 08:53:32 DEBUG    rasa.nlu.classifiers.diet_classifier  -   t_loss (total loss)
2025-06-03 08:53:32 DEBUG    rasa.nlu.classifiers.diet_classifier  -   i_acc (intent acc)
2025-06-03 08:53:32 DEBUG    rasa.nlu.classifiers.diet_classifier  -   i_loss (intent loss)
2025-06-03 08:53:41 DEBUG    rasa.utils.tensorflow.models  - Finished loading the model.
2025-06-03 08:53:41 DEBUG    rasa.engine.graph  - Node 'run_EntitySynonymMapper6' loading 'EntitySynonymMapper.load' and kwargs: '{}'.
2025-06-03 08:53:41 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_EntitySynonymMapper6' was requested for reading.
2025-06-03 08:53:41 DEBUG    rasa.nlu.extractors.entity_synonyms  - Failed to load ABCMeta from model storage. Resource 'train_EntitySynonymMapper6' doesn't exist.
2025-06-03 08:53:41 DEBUG    rasa.engine.graph  - Node 'run_ResponseSelector7' loading 'ResponseSelector.load' and kwargs: '{}'.
2025-06-03 08:53:41 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_ResponseSelector7' was requested for reading.
2025-06-03 08:53:41 DEBUG    rasa.nlu.classifiers.diet_classifier  - Failed to load ABCMeta from model storage. Resource 'train_ResponseSelector7' doesn't exist.
2025-06-03 08:53:41 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_ResponseSelector7' was requested for reading.
2025-06-03 08:53:41 DEBUG    rasa.nlu.selectors.response_selector  - Failed to load ResponseSelector from model storage. Resource 'train_ResponseSelector7' doesn't exist.
2025-06-03 08:53:41 DEBUG    rasa.engine.graph  - Node 'run_FallbackClassifier8' loading 'FallbackClassifier.load' and kwargs: '{}'.
2025-06-03 08:53:41 DEBUG    rasa.engine.graph  - Node 'run_RegexMessageHandler' loading 'RegexMessageHandler.load' and kwargs: '{}'.
2025-06-03 08:53:41 DEBUG    rasa.engine.graph  - Node 'domain_provider' loading 'DomainProvider.load' and kwargs: '{}'.
2025-06-03 08:53:41 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'domain_provider' was requested for reading.
2025-06-03 08:53:41 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' loading 'MemoizationPolicy.load' and kwargs: '{}'.
2025-06-03 08:53:41 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_MemoizationPolicy0' was requested for reading.
2025-06-03 08:53:41 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy1' loading 'TEDPolicy.load' and kwargs: '{}'.
2025-06-03 08:53:41 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_TEDPolicy1' was requested for reading.
2025-06-03 08:53:41 DEBUG    rasa.utils.tensorflow.models  - Loading the model from /var/folders/mn/468p6dp91qb8p_yc3wtlxkv40000gp/T/tmpkcqdo7o0/train_TEDPolicy1/ted_policy.tf_model with finetune_mode=False...
2025-06-03 08:53:50 DEBUG    rasa.utils.tensorflow.models  - Finished loading the model.
2025-06-03 08:53:50 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy2' loading 'RulePolicy.load' and kwargs: '{}'.
2025-06-03 08:53:50 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_RulePolicy2' was requested for reading.
2025-06-03 08:53:50 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' loading 'RuleOnlyDataProvider.load' and kwargs: '{}'.
2025-06-03 08:53:50 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_RulePolicy2' was requested for reading.
2025-06-03 08:53:50 DEBUG    rasa.engine.graph  - Node 'select_prediction' loading 'DefaultPolicyPredictionEnsemble.load' and kwargs: '{}'.
2025-06-03 08:53:50 INFO     root  - Rasa server is up and running.
2025-06-03 08:53:50 INFO     root  - Enabling coroutine debugging. Loop id 140472024563728.
2025-06-03 08:55:11 DEBUG    rasa.core.lock_store  - Issuing ticket for conversation 'PractikumStudent'.
2025-06-03 08:55:11 DEBUG    rasa.core.lock_store  - Acquiring lock for conversation 'PractikumStudent'.
2025-06-03 08:55:11 DEBUG    rasa.core.lock_store  - Acquired lock for conversation 'PractikumStudent'.
2025-06-03 08:55:11 DEBUG    rasa.core.tracker_store  - Could not find tracker for conversation ID 'PractikumStudent'.
2025-06-03 08:55:11 DEBUG    rasa.core.tracker_store  - No event broker configured. Skipping streaming events.
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - Starting a new session for conversation ID 'PractikumStudent'.
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[]
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=action_session_start rasa_events=[<rasa.shared.core.events.SessionStarted object at 0x7fc21eb4ddc0>, ActionExecuted(action: action_listen, policy: None, confidence: None)]
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - [debug    ] processor.slots.log            slot_values=	session_started_metadata: None
2025-06-03 08:55:11 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__message__': [<rasa.core.channels.channel.UserMessage object at 0x7fc239cc82e0>], '__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf91bb0>}, targets: ['run_RegexMessageHandler'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'nlu_message_converter' running 'NLUMessageConverter.convert_user_message'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_WhitespaceTokenizer0' running 'WhitespaceTokenizer.process'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_RegexFeaturizer1' running 'RegexFeaturizer.process'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_LexicalSyntacticFeaturizer2' running 'LexicalSyntacticFeaturizer.process'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer3' running 'CountVectorsFeaturizer.process'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer4' running 'CountVectorsFeaturizer.process'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_DIETClassifier5' running 'DIETClassifier.process'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_EntitySynonymMapper6' running 'EntitySynonymMapper.process'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_ResponseSelector7' running 'ResponseSelector.process'.
2025-06-03 08:55:11 DEBUG    rasa.nlu.classifiers.diet_classifier  - There is no trained model for 'ResponseSelector': The component is either not trained or didn't receive enough training data.
2025-06-03 08:55:11 DEBUG    rasa.nlu.selectors.response_selector  - Adding following selector key to message property: default
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_FallbackClassifier8' running 'FallbackClassifier.process'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_RegexMessageHandler' running 'RegexMessageHandler.process'.
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - [debug    ] processor.message.parse        parse_data_entities=[] parse_data_intent={'name': 'greet', 'confidence': 0.9998708963394165} parse_data_text=Привет!
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - Logged UserUtterance - tracker now has 4 events.
2025-06-03 08:55:11 DEBUG    rasa.core.actions.action  - Validating extracted slots:
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - [debug    ] processor.extract.slots        action_extract_slot=action_extract_slots len_extraction_events=0 rasa_events=[]
2025-06-03 08:55:11 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf91bb0>}, targets: ['select_prediction'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2025-06-03 08:55:11 DEBUG    rasa.core.policies.memoization  - [debug    ] memoization.predict.actions    tracker_states=[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}]
2025-06-03 08:55:11 DEBUG    rasa.core.policies.memoization  - There is a memorised next action 'utter_greet'
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy2' running 'RulePolicy.predict_action_probabilities'.
2025-06-03 08:55:11 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user text: Привет! | previous action name: action_listen
2025-06-03 08:55:11 DEBUG    rasa.core.policies.rule_policy  - There is no applicable rule.
2025-06-03 08:55:11 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
2025-06-03 08:55:11 DEBUG    rasa.core.policies.rule_policy  - There is a rule for the next action 'utter_greet'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy1' running 'TEDPolicy.predict_action_probabilities'.
2025-06-03 08:55:11 DEBUG    rasa.core.policies.ted_policy  - TED predicted 'utter_greet' based on user intent.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2025-06-03 08:55:11 DEBUG    rasa.core.policies.ensemble  - Made prediction using user intent.
2025-06-03 08:55:11 DEBUG    rasa.core.policies.ensemble  - Added `DefinePrevUserUtteredFeaturization(False)` event.
2025-06-03 08:55:11 DEBUG    rasa.core.policies.ensemble  - Predicted next action using RulePolicy.
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - Predicted next action 'utter_greet' with confidence 1.00.
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[<rasa.shared.core.events.DefinePrevUserUtteredFeaturization object at 0x7fc21eb4d220>]
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=utter_greet rasa_events=[BotUttered('Привет! Я ассистент по архитектуре ПО. Чем могу помочь?', {"elements": null, "quick_replies": null, "buttons": null, "attachment": null, "image": null, "custom": null}, {"utter_action": "utter_greet"}, 1748930111.386411)]
2025-06-03 08:55:11 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf91bb0>}, targets: ['select_prediction'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2025-06-03 08:55:11 DEBUG    rasa.core.policies.memoization  - [debug    ] memoization.predict.actions    tracker_states=[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}]
2025-06-03 08:55:11 DEBUG    rasa.core.policies.memoization  - There is a memorised next action 'action_listen'
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy2' running 'RulePolicy.predict_action_probabilities'.
2025-06-03 08:55:11 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
2025-06-03 08:55:11 DEBUG    rasa.core.policies.rule_policy  - There is a rule for the next action 'action_listen'.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy1' running 'TEDPolicy.predict_action_probabilities'.
2025-06-03 08:55:11 DEBUG    rasa.core.policies.ted_policy  - TED predicted 'action_listen' based on user intent.
2025-06-03 08:55:11 DEBUG    rasa.engine.graph  - Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2025-06-03 08:55:11 DEBUG    rasa.core.policies.ensemble  - Predicted next action using RulePolicy.
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - Predicted next action 'action_listen' with confidence 1.00.
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[]
2025-06-03 08:55:11 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=action_listen rasa_events=[]
2025-06-03 08:55:11 DEBUG    rasa.core.tracker_store  - No event broker configured. Skipping streaming events.
2025-06-03 08:55:11 DEBUG    rasa.core.lock_store  - Deleted lock for conversation 'PractikumStudent'.
2025-06-03 08:55:24 DEBUG    rasa.core.lock_store  - Issuing ticket for conversation 'PractikumStudent'.
2025-06-03 08:55:24 DEBUG    rasa.core.lock_store  - Acquiring lock for conversation 'PractikumStudent'.
2025-06-03 08:55:24 DEBUG    rasa.core.lock_store  - Acquired lock for conversation 'PractikumStudent'.
2025-06-03 08:55:24 DEBUG    rasa.core.tracker_store  - Recreating tracker for id 'PractikumStudent'
2025-06-03 08:55:24 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__message__': [<rasa.core.channels.channel.UserMessage object at 0x7fc231292be0>], '__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf918e0>}, targets: ['run_RegexMessageHandler'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'nlu_message_converter' running 'NLUMessageConverter.convert_user_message'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_WhitespaceTokenizer0' running 'WhitespaceTokenizer.process'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_RegexFeaturizer1' running 'RegexFeaturizer.process'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_LexicalSyntacticFeaturizer2' running 'LexicalSyntacticFeaturizer.process'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer3' running 'CountVectorsFeaturizer.process'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer4' running 'CountVectorsFeaturizer.process'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_DIETClassifier5' running 'DIETClassifier.process'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_EntitySynonymMapper6' running 'EntitySynonymMapper.process'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_ResponseSelector7' running 'ResponseSelector.process'.
2025-06-03 08:55:24 DEBUG    rasa.nlu.classifiers.diet_classifier  - There is no trained model for 'ResponseSelector': The component is either not trained or didn't receive enough training data.
2025-06-03 08:55:24 DEBUG    rasa.nlu.selectors.response_selector  - Adding following selector key to message property: default
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_FallbackClassifier8' running 'FallbackClassifier.process'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_RegexMessageHandler' running 'RegexMessageHandler.process'.
2025-06-03 08:55:24 DEBUG    rasa.core.processor  - [debug    ] processor.message.parse        parse_data_entities=[] parse_data_intent={'name': 'ask_monolith', 'confidence': 0.9790946841239929} parse_data_text=Что такое монолитная архитектура?
2025-06-03 08:55:24 DEBUG    rasa.core.processor  - Logged UserUtterance - tracker now has 9 events.
2025-06-03 08:55:24 DEBUG    rasa.core.actions.action  - Validating extracted slots:
2025-06-03 08:55:24 DEBUG    rasa.core.processor  - [debug    ] processor.extract.slots        action_extract_slot=action_extract_slots len_extraction_events=0 rasa_events=[]
2025-06-03 08:55:24 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf918e0>}, targets: ['select_prediction'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2025-06-03 08:55:24 DEBUG    rasa.core.policies.memoization  - [debug    ] memoization.predict.actions    tracker_states=[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}, {'user': {'intent': 'ask_monolith'}, 'prev_action': {'action_name': 'action_listen'}}]
2025-06-03 08:55:24 DEBUG    rasa.core.policies.memoization  - There is no memorised next action
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy2' running 'RulePolicy.predict_action_probabilities'.
2025-06-03 08:55:24 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user text: Что такое монолитная архитектура? | previous action name: action_listen
2025-06-03 08:55:24 DEBUG    rasa.core.policies.rule_policy  - There is no applicable rule.
2025-06-03 08:55:24 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user intent: ask_monolith | previous action name: action_listen
2025-06-03 08:55:24 DEBUG    rasa.core.policies.rule_policy  - There is a rule for the next action 'utter_ask_monolith'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy1' running 'TEDPolicy.predict_action_probabilities'.
2025-06-03 08:55:24 DEBUG    rasa.core.policies.ted_policy  - TED predicted 'action_listen' based on user intent.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2025-06-03 08:55:24 DEBUG    rasa.core.policies.ensemble  - Made prediction using user intent.
2025-06-03 08:55:24 DEBUG    rasa.core.policies.ensemble  - Added `DefinePrevUserUtteredFeaturization(False)` event.
2025-06-03 08:55:24 DEBUG    rasa.core.policies.ensemble  - Predicted next action using RulePolicy.
2025-06-03 08:55:24 DEBUG    rasa.core.processor  - Predicted next action 'utter_ask_monolith' with confidence 1.00.
2025-06-03 08:55:24 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[<rasa.shared.core.events.DefinePrevUserUtteredFeaturization object at 0x7fc21eb4d160>]
2025-06-03 08:55:24 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=utter_ask_monolith rasa_events=[BotUttered('Монолит - единое приложение, где все компоненты связаны. Плюсы: простота разработки. Минусы: сложность масштабирования.', {"elements": null, "quick_replies": null, "buttons": null, "attachment": null, "image": null, "custom": null}, {"utter_action": "utter_ask_monolith"}, 1748930124.276886)]
2025-06-03 08:55:24 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf918e0>}, targets: ['select_prediction'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2025-06-03 08:55:24 DEBUG    rasa.core.policies.memoization  - [debug    ] memoization.predict.actions    tracker_states=[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}]
2025-06-03 08:55:24 DEBUG    rasa.core.policies.memoization  - There is no memorised next action
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy2' running 'RulePolicy.predict_action_probabilities'.
2025-06-03 08:55:24 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user intent: ask_monolith | previous action name: action_listen
[state 4] user intent: ask_monolith | previous action name: utter_ask_monolith
2025-06-03 08:55:24 DEBUG    rasa.core.policies.rule_policy  - There is a rule for the next action 'action_listen'.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy1' running 'TEDPolicy.predict_action_probabilities'.
2025-06-03 08:55:24 DEBUG    rasa.core.policies.ted_policy  - TED predicted 'utter_greet' based on user intent.
2025-06-03 08:55:24 DEBUG    rasa.engine.graph  - Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2025-06-03 08:55:24 DEBUG    rasa.core.policies.ensemble  - Predicted next action using RulePolicy.
2025-06-03 08:55:24 DEBUG    rasa.core.processor  - Predicted next action 'action_listen' with confidence 1.00.
2025-06-03 08:55:24 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[]
2025-06-03 08:55:24 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=action_listen rasa_events=[]
2025-06-03 08:55:24 DEBUG    rasa.core.tracker_store  - No event broker configured. Skipping streaming events.
2025-06-03 08:55:24 DEBUG    rasa.core.lock_store  - Deleted lock for conversation 'PractikumStudent'.
2025-06-03 08:56:15 DEBUG    rasa.core.lock_store  - Issuing ticket for conversation 'PractikumStudent'.
2025-06-03 08:56:15 DEBUG    rasa.core.lock_store  - Acquiring lock for conversation 'PractikumStudent'.
2025-06-03 08:56:15 DEBUG    rasa.core.lock_store  - Acquired lock for conversation 'PractikumStudent'.
2025-06-03 08:56:15 DEBUG    rasa.core.tracker_store  - Recreating tracker for id 'PractikumStudent'
2025-06-03 08:56:15 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__message__': [<rasa.core.channels.channel.UserMessage object at 0x7fc239d3c9d0>], '__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf918e0>}, targets: ['run_RegexMessageHandler'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'nlu_message_converter' running 'NLUMessageConverter.convert_user_message'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_WhitespaceTokenizer0' running 'WhitespaceTokenizer.process'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_RegexFeaturizer1' running 'RegexFeaturizer.process'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_LexicalSyntacticFeaturizer2' running 'LexicalSyntacticFeaturizer.process'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer3' running 'CountVectorsFeaturizer.process'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer4' running 'CountVectorsFeaturizer.process'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_DIETClassifier5' running 'DIETClassifier.process'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_EntitySynonymMapper6' running 'EntitySynonymMapper.process'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_ResponseSelector7' running 'ResponseSelector.process'.
2025-06-03 08:56:15 DEBUG    rasa.nlu.classifiers.diet_classifier  - There is no trained model for 'ResponseSelector': The component is either not trained or didn't receive enough training data.
2025-06-03 08:56:15 DEBUG    rasa.nlu.selectors.response_selector  - Adding following selector key to message property: default
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_FallbackClassifier8' running 'FallbackClassifier.process'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_RegexMessageHandler' running 'RegexMessageHandler.process'.
2025-06-03 08:56:15 DEBUG    rasa.core.processor  - [debug    ] processor.message.parse        parse_data_entities=[] parse_data_intent={'name': 'ask_microservices', 'confidence': 0.8789326548576355} parse_data_text=Что такое микросервисная архитектура?
2025-06-03 08:56:15 DEBUG    rasa.core.processor  - Logged UserUtterance - tracker now has 14 events.
2025-06-03 08:56:15 DEBUG    rasa.core.actions.action  - Validating extracted slots:
2025-06-03 08:56:15 DEBUG    rasa.core.processor  - [debug    ] processor.extract.slots        action_extract_slot=action_extract_slots len_extraction_events=0 rasa_events=[]
2025-06-03 08:56:15 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf918e0>}, targets: ['select_prediction'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2025-06-03 08:56:15 DEBUG    rasa.core.policies.memoization  - [debug    ] memoization.predict.actions    tracker_states=[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}, {'user': {'intent': 'ask_microservices'}, 'prev_action': {'action_name': 'action_listen'}}]
2025-06-03 08:56:15 DEBUG    rasa.core.policies.memoization  - There is a memorised next action 'utter_ask_microservices'
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy2' running 'RulePolicy.predict_action_probabilities'.
2025-06-03 08:56:15 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user intent: ask_monolith | previous action name: action_listen
[state 4] user intent: ask_monolith | previous action name: utter_ask_monolith
[state 5] user text: Что такое микросервисная архитектура? | previous action name: action_listen
2025-06-03 08:56:15 DEBUG    rasa.core.policies.rule_policy  - There is no applicable rule.
2025-06-03 08:56:15 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user intent: ask_monolith | previous action name: action_listen
[state 4] user intent: ask_monolith | previous action name: utter_ask_monolith
[state 5] user intent: ask_microservices | previous action name: action_listen
2025-06-03 08:56:15 DEBUG    rasa.core.policies.rule_policy  - There is a rule for the next action 'utter_ask_microservices'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy1' running 'TEDPolicy.predict_action_probabilities'.
2025-06-03 08:56:15 DEBUG    rasa.core.policies.ted_policy  - TED predicted 'utter_ask_microservices' based on user intent.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2025-06-03 08:56:15 DEBUG    rasa.core.policies.ensemble  - Made prediction using user intent.
2025-06-03 08:56:15 DEBUG    rasa.core.policies.ensemble  - Added `DefinePrevUserUtteredFeaturization(False)` event.
2025-06-03 08:56:15 DEBUG    rasa.core.policies.ensemble  - Predicted next action using RulePolicy.
2025-06-03 08:56:15 DEBUG    rasa.core.processor  - Predicted next action 'utter_ask_microservices' with confidence 1.00.
2025-06-03 08:56:15 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[<rasa.shared.core.events.DefinePrevUserUtteredFeaturization object at 0x7fc21eb4d1f0>]
2025-06-03 08:56:15 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=utter_ask_microservices rasa_events=[BotUttered('Микросервисы - это архитектурный стиль, где приложение состоит из небольших независимых сервисов. Плюсы: масштабируемость, гибкость. Минусы: сложность, overhead.', {"elements": null, "quick_replies": null, "buttons": null, "attachment": null, "image": null, "custom": null}, {"utter_action": "utter_ask_microservices"}, 1748930175.777426)]
2025-06-03 08:56:15 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf918e0>}, targets: ['select_prediction'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2025-06-03 08:56:15 DEBUG    rasa.core.policies.memoization  - [debug    ] memoization.predict.actions    tracker_states=[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}, {'user': {'intent': 'ask_microservices'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'ask_microservices'}, 'prev_action': {'action_name': 'utter_ask_microservices'}}]
2025-06-03 08:56:15 DEBUG    rasa.core.policies.memoization  - There is a memorised next action 'action_listen'
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy2' running 'RulePolicy.predict_action_probabilities'.
2025-06-03 08:56:15 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user intent: ask_monolith | previous action name: action_listen
[state 4] user intent: ask_monolith | previous action name: utter_ask_monolith
[state 5] user intent: ask_microservices | previous action name: action_listen
[state 6] user intent: ask_microservices | previous action name: utter_ask_microservices
2025-06-03 08:56:15 DEBUG    rasa.core.policies.rule_policy  - There is a rule for the next action 'action_listen'.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy1' running 'TEDPolicy.predict_action_probabilities'.
2025-06-03 08:56:15 DEBUG    rasa.core.policies.ted_policy  - TED predicted 'action_listen' based on user intent.
2025-06-03 08:56:15 DEBUG    rasa.engine.graph  - Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2025-06-03 08:56:15 DEBUG    rasa.core.policies.ensemble  - Predicted next action using RulePolicy.
2025-06-03 08:56:15 DEBUG    rasa.core.processor  - Predicted next action 'action_listen' with confidence 1.00.
2025-06-03 08:56:15 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[]
2025-06-03 08:56:15 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=action_listen rasa_events=[]
2025-06-03 08:56:15 DEBUG    rasa.core.tracker_store  - No event broker configured. Skipping streaming events.
2025-06-03 08:56:15 DEBUG    rasa.core.lock_store  - Deleted lock for conversation 'PractikumStudent'.
2025-06-03 08:59:17 DEBUG    rasa.core.lock_store  - Issuing ticket for conversation 'PractikumStudent'.
2025-06-03 08:59:17 DEBUG    rasa.core.lock_store  - Acquiring lock for conversation 'PractikumStudent'.
2025-06-03 08:59:17 DEBUG    rasa.core.lock_store  - Acquired lock for conversation 'PractikumStudent'.
2025-06-03 08:59:17 DEBUG    rasa.core.tracker_store  - Recreating tracker for id 'PractikumStudent'
2025-06-03 08:59:17 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__message__': [<rasa.core.channels.channel.UserMessage object at 0x7fc231292bb0>], '__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf918e0>}, targets: ['run_RegexMessageHandler'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'nlu_message_converter' running 'NLUMessageConverter.convert_user_message'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_WhitespaceTokenizer0' running 'WhitespaceTokenizer.process'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_RegexFeaturizer1' running 'RegexFeaturizer.process'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_LexicalSyntacticFeaturizer2' running 'LexicalSyntacticFeaturizer.process'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer3' running 'CountVectorsFeaturizer.process'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer4' running 'CountVectorsFeaturizer.process'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_DIETClassifier5' running 'DIETClassifier.process'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_EntitySynonymMapper6' running 'EntitySynonymMapper.process'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_ResponseSelector7' running 'ResponseSelector.process'.
2025-06-03 08:59:17 DEBUG    rasa.nlu.classifiers.diet_classifier  - There is no trained model for 'ResponseSelector': The component is either not trained or didn't receive enough training data.
2025-06-03 08:59:17 DEBUG    rasa.nlu.selectors.response_selector  - Adding following selector key to message property: default
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_FallbackClassifier8' running 'FallbackClassifier.process'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_RegexMessageHandler' running 'RegexMessageHandler.process'.
2025-06-03 08:59:17 DEBUG    rasa.core.processor  - [debug    ] processor.message.parse        parse_data_entities=[] parse_data_intent={'name': 'thanks', 'confidence': 0.9998500347137451} parse_data_text=Спасибо!
2025-06-03 08:59:17 DEBUG    rasa.core.processor  - Logged UserUtterance - tracker now has 19 events.
2025-06-03 08:59:17 DEBUG    rasa.core.actions.action  - Validating extracted slots:
2025-06-03 08:59:17 DEBUG    rasa.core.processor  - [debug    ] processor.extract.slots        action_extract_slot=action_extract_slots len_extraction_events=0 rasa_events=[]
2025-06-03 08:59:17 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf918e0>}, targets: ['select_prediction'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2025-06-03 08:59:17 DEBUG    rasa.core.policies.memoization  - [debug    ] memoization.predict.actions    tracker_states=[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}, {'user': {'intent': 'ask_microservices'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'ask_microservices'}, 'prev_action': {'action_name': 'utter_ask_microservices'}}, {'user': {'intent': 'thanks'}, 'prev_action': {'action_name': 'action_listen'}}]
2025-06-03 08:59:17 DEBUG    rasa.core.policies.memoization  - There is no memorised next action
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy2' running 'RulePolicy.predict_action_probabilities'.
2025-06-03 08:59:17 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user intent: ask_monolith | previous action name: action_listen
[state 4] user intent: ask_monolith | previous action name: utter_ask_monolith
[state 5] user intent: ask_microservices | previous action name: action_listen
[state 6] user intent: ask_microservices | previous action name: utter_ask_microservices
[state 7] user text: Спасибо! | previous action name: action_listen
2025-06-03 08:59:17 DEBUG    rasa.core.policies.rule_policy  - There is no applicable rule.
2025-06-03 08:59:17 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user intent: ask_monolith | previous action name: action_listen
[state 4] user intent: ask_monolith | previous action name: utter_ask_monolith
[state 5] user intent: ask_microservices | previous action name: action_listen
[state 6] user intent: ask_microservices | previous action name: utter_ask_microservices
[state 7] user intent: thanks | previous action name: action_listen
2025-06-03 08:59:17 DEBUG    rasa.core.policies.rule_policy  - There is a rule for the next action 'utter_thanks'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy1' running 'TEDPolicy.predict_action_probabilities'.
2025-06-03 08:59:17 DEBUG    rasa.core.policies.ted_policy  - TED predicted 'utter_thanks' based on user intent.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2025-06-03 08:59:17 DEBUG    rasa.core.policies.ensemble  - Made prediction using user intent.
2025-06-03 08:59:17 DEBUG    rasa.core.policies.ensemble  - Added `DefinePrevUserUtteredFeaturization(False)` event.
2025-06-03 08:59:17 DEBUG    rasa.core.policies.ensemble  - Predicted next action using RulePolicy.
2025-06-03 08:59:17 DEBUG    rasa.core.processor  - Predicted next action 'utter_thanks' with confidence 1.00.
2025-06-03 08:59:17 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[<rasa.shared.core.events.DefinePrevUserUtteredFeaturization object at 0x7fc220264580>]
2025-06-03 08:59:17 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=utter_thanks rasa_events=[BotUttered('Пожалуйста! Обращайтесь, если нужна помощь.', {"elements": null, "quick_replies": null, "buttons": null, "attachment": null, "image": null, "custom": null}, {"utter_action": "utter_thanks"}, 1748930357.5375009)]
2025-06-03 08:59:17 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7fc21cf918e0>}, targets: ['select_prediction'] and ExecutionContext(model_id='e08284da7e0a44d580c29565d76d67f1', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2025-06-03 08:59:17 DEBUG    rasa.core.policies.memoization  - [debug    ] memoization.predict.actions    tracker_states=[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}, {'user': {'intent': 'ask_microservices'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'ask_microservices'}, 'prev_action': {'action_name': 'utter_ask_microservices'}}, {'user': {'intent': 'thanks'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'thanks'}, 'prev_action': {'action_name': 'utter_thanks'}}]
2025-06-03 08:59:17 DEBUG    rasa.core.policies.memoization  - There is no memorised next action
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy2' running 'RulePolicy.predict_action_probabilities'.
2025-06-03 08:59:17 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user intent: ask_monolith | previous action name: action_listen
[state 4] user intent: ask_monolith | previous action name: utter_ask_monolith
[state 5] user intent: ask_microservices | previous action name: action_listen
[state 6] user intent: ask_microservices | previous action name: utter_ask_microservices
[state 7] user intent: thanks | previous action name: action_listen
[state 8] user intent: thanks | previous action name: utter_thanks
2025-06-03 08:59:17 DEBUG    rasa.core.policies.rule_policy  - There is a rule for the next action 'action_listen'.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy1' running 'TEDPolicy.predict_action_probabilities'.
2025-06-03 08:59:17 DEBUG    rasa.core.policies.ted_policy  - TED predicted 'action_listen' based on user intent.
2025-06-03 08:59:17 DEBUG    rasa.engine.graph  - Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2025-06-03 08:59:17 DEBUG    rasa.core.policies.ensemble  - Predicted next action using RulePolicy.
2025-06-03 08:59:17 DEBUG    rasa.core.processor  - Predicted next action 'action_listen' with confidence 1.00.
2025-06-03 08:59:17 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[]
2025-06-03 08:59:17 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=action_listen rasa_events=[]
2025-06-03 08:59:17 DEBUG    rasa.core.tracker_store  - No event broker configured. Skipping streaming events.
2025-06-03 08:59:17 DEBUG    rasa.core.lock_store  - Deleted lock for conversation 'PractikumStudent'.
```
