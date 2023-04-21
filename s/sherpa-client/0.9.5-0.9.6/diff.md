# Comparing `tmp/sherpa-client-0.9.5.tar.gz` & `tmp/sherpa-client-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-client-0.9.5.tar", last modified: Thu Dec  2 12:58:03 2021, max compression
+gzip compressed data, was "sherpa-client-0.9.6.tar", last modified: Thu Dec  2 13:42:09 2021, max compression
```

## Comparing `sherpa-client-0.9.5.tar` & `sherpa-client-0.9.6.tar`

### file list

```diff
@@ -1,377 +1,377 @@
--rw-r--r--   0        0        0    11357 2021-12-02 10:16:57.780981 sherpa-client-0.9.5/LICENSE
--rw-r--r--   0        0        0     3606 2021-12-02 09:15:30.387702 sherpa-client-0.9.5/README.md
--rw-r--r--   0        0        0      825 2021-12-02 12:57:55.095456 sherpa-client-0.9.5/pyproject.toml
--rw-r--r--   0        0        0      112 2021-12-02 09:15:38.135674 sherpa-client-0.9.5/sherpa_client/__init__.py
--rw-r--r--   0        0        0       47 2021-12-02 09:15:38.131674 sherpa-client-0.9.5/sherpa_client/api/__init__.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.579702 sherpa-client-0.9.5/sherpa_client/api/annotate/__init__.py
--rw-r--r--   0        0        0     4860 2021-12-02 09:15:38.363674 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_binary.py
--rw-r--r--   0        0        0     5574 2021-12-02 09:15:38.383674 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_binary_with_plan_ref.py
--rw-r--r--   0        0        0     3581 2021-12-02 09:15:38.323674 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_corpus_with.py
--rw-r--r--   0        0        0     5581 2021-12-02 09:15:38.395673 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_documents_with.py
--rw-r--r--   0        0        0     4817 2021-12-02 09:15:38.363674 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_documents_with_many.py
--rw-r--r--   0        0        0     3910 2021-12-02 09:15:38.319674 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_binary.py
--rw-r--r--   0        0        0     4681 2021-12-02 09:15:38.363674 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_binary_with_plan_ref.py
--rw-r--r--   0        0        0     3867 2021-12-02 09:15:38.359674 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_documents_with_many.py
--rw-r--r--   0        0        0     4644 2021-12-02 09:15:38.367673 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_documents_with_plan_ref.py
--rw-r--r--   0        0        0     3827 2021-12-02 09:15:38.347674 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_text_with_many.py
--rw-r--r--   0        0        0     3965 2021-12-02 09:15:38.403674 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_text_with_plan_ref.py
--rw-r--r--   0        0        0     4246 2021-12-02 09:15:38.383674 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_text.py
--rw-r--r--   0        0        0     4524 2021-12-02 09:15:38.583673 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_text_with.py
--rw-r--r--   0        0        0     4398 2021-12-02 09:15:38.559673 sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_text_with_many.py
--rw-r--r--   0        0        0     3901 2021-12-02 09:15:38.551673 sherpa-client-0.9.5/sherpa_client/api/annotate/format_binary.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.575701 sherpa-client-0.9.5/sherpa_client/api/annotations/__init__.py
--rw-r--r--   0        0        0     2623 2021-12-02 09:15:38.547673 sherpa-client-0.9.5/sherpa_client/api/annotations/annotation_creators_count.py
--rw-r--r--   0        0        0     3661 2021-12-02 09:15:38.579673 sherpa-client-0.9.5/sherpa_client/api/annotations/clear_annotations.py
--rw-r--r--   0        0        0     3661 2021-12-02 09:15:38.571673 sherpa-client-0.9.5/sherpa_client/api/annotations/count_annotations.py
--rw-r--r--   0        0        0     2590 2021-12-02 09:15:38.503673 sherpa-client-0.9.5/sherpa_client/api/annotations/create_annotation.py
--rw-r--r--   0        0        0     2546 2021-12-02 09:15:38.563673 sherpa-client-0.9.5/sherpa_client/api/annotations/delete_annotation.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.611701 sherpa-client-0.9.5/sherpa_client/api/annotators/__init__.py
--rw-r--r--   0        0        0     2267 2021-12-02 09:15:38.515673 sherpa-client-0.9.5/sherpa_client/api/annotators/get_annotators_by_type.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.531702 sherpa-client-0.9.5/sherpa_client/api/authentication/__init__.py
--rw-r--r--   0        0        0     4771 2021-12-02 09:15:38.635673 sherpa-client-0.9.5/sherpa_client/api/authentication/request_jwt_token.py
--rw-r--r--   0        0        0     1243 2021-12-02 09:15:38.467673 sherpa-client-0.9.5/sherpa_client/api/authentication/user_sign_out.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.603701 sherpa-client-0.9.5/sherpa_client/api/categories/__init__.py
--rw-r--r--   0        0        0     2622 2021-12-02 09:15:38.547673 sherpa-client-0.9.5/sherpa_client/api/categories/category_creators_count.py
--rw-r--r--   0        0        0     3660 2021-12-02 09:15:38.679672 sherpa-client-0.9.5/sherpa_client/api/categories/count_categories.py
--rw-r--r--   0        0        0     2557 2021-12-02 09:15:38.639673 sherpa-client-0.9.5/sherpa_client/api/categories/create_document_category.py
--rw-r--r--   0        0        0     3660 2021-12-02 09:15:38.739672 sherpa-client-0.9.5/sherpa_client/api/categories/delete_categories.py
--rw-r--r--   0        0        0     2671 2021-12-02 09:15:38.707672 sherpa-client-0.9.5/sherpa_client/api/categories/delete_category.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.631701 sherpa-client-0.9.5/sherpa_client/api/documents/__init__.py
--rw-r--r--   0        0        0     2512 2021-12-02 09:15:38.715672 sherpa-client-0.9.5/sherpa_client/api/documents/delete_document.py
--rw-r--r--   0        0        0     3416 2021-12-02 09:15:38.771672 sherpa-client-0.9.5/sherpa_client/api/documents/export_documents.py
--rw-r--r--   0        0        0     3069 2021-12-02 09:15:38.739672 sherpa-client-0.9.5/sherpa_client/api/documents/export_documents_sample.py
--rw-r--r--   0        0        0     3604 2021-12-02 09:15:38.803672 sherpa-client-0.9.5/sherpa_client/api/documents/get_document.py
--rw-r--r--   0        0        0     2529 2021-12-02 09:15:38.719672 sherpa-client-0.9.5/sherpa_client/api/documents/index_document.py
--rw-r--r--   0        0        0     6566 2021-12-02 09:15:38.891672 sherpa-client-0.9.5/sherpa_client/api/documents/launch_document_import.py
--rw-r--r--   0        0        0     6698 2021-12-02 09:15:38.931671 sherpa-client-0.9.5/sherpa_client/api/documents/launch_uploaded_document_import.py
--rw-r--r--   0        0        0     4802 2021-12-02 09:15:38.931671 sherpa-client-0.9.5/sherpa_client/api/documents/search_and_delete_documents.py
--rw-r--r--   0        0        0     5058 2021-12-02 09:15:38.943672 sherpa-client-0.9.5/sherpa_client/api/documents/search_and_export_documents.py
--rw-r--r--   0        0        0     5201 2021-12-02 09:15:38.983671 sherpa-client-0.9.5/sherpa_client/api/documents/search_and_tag_documents.py
--rw-r--r--   0        0        0     6569 2021-12-02 09:15:39.159671 sherpa-client-0.9.5/sherpa_client/api/documents/search_documents.py
--rw-r--r--   0        0        0     2025 2021-12-02 09:15:38.843672 sherpa-client-0.9.5/sherpa_client/api/documents/set_metadata_on_document.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.647701 sherpa-client-0.9.5/sherpa_client/api/experiments/__init__.py
--rw-r--r--   0        0        0     1554 2021-12-02 09:15:38.815672 sherpa-client-0.9.5/sherpa_client/api/experiments/cancel_experiment.py
--rw-r--r--   0        0        0     2658 2021-12-02 09:15:38.891672 sherpa-client-0.9.5/sherpa_client/api/experiments/compute_experiment_label_hint.py
--rw-r--r--   0        0        0     2594 2021-12-02 09:15:38.875672 sherpa-client-0.9.5/sherpa_client/api/experiments/create_experiment.py
--rw-r--r--   0        0        0     2584 2021-12-02 09:15:38.923672 sherpa-client-0.9.5/sherpa_client/api/experiments/delete_experiment.py
--rw-r--r--   0        0        0     2585 2021-12-02 09:15:38.979671 sherpa-client-0.9.5/sherpa_client/api/experiments/delete_experiments.py
--rw-r--r--   0        0        0     2541 2021-12-02 09:15:39.039671 sherpa-client-0.9.5/sherpa_client/api/experiments/get_experiment.py
--rw-r--r--   0        0        0     2513 2021-12-02 09:15:39.003671 sherpa-client-0.9.5/sherpa_client/api/experiments/get_experiments.py
--rw-r--r--   0        0        0     2594 2021-12-02 09:15:39.039671 sherpa-client-0.9.5/sherpa_client/api/experiments/launch_experiment.py
--rw-r--r--   0        0        0     2545 2021-12-02 09:15:39.035671 sherpa-client-0.9.5/sherpa_client/api/experiments/patch_experiment.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.659701 sherpa-client-0.9.5/sherpa_client/api/gazetteers/__init__.py
--rw-r--r--   0        0        0     1565 2021-12-02 09:15:38.983671 sherpa-client-0.9.5/sherpa_client/api/gazetteers/cancel_synchronize_gazetteer.py
--rw-r--r--   0        0        0     2657 2021-12-02 09:15:39.083671 sherpa-client-0.9.5/sherpa_client/api/gazetteers/compute_gazetteer_label_hint.py
--rw-r--r--   0        0        0     2586 2021-12-02 09:15:39.071671 sherpa-client-0.9.5/sherpa_client/api/gazetteers/create_gazetteer.py
--rw-r--r--   0        0        0     2583 2021-12-02 09:15:39.131671 sherpa-client-0.9.5/sherpa_client/api/gazetteers/delete_gazetteer.py
--rw-r--r--   0        0        0     2584 2021-12-02 09:15:39.087671 sherpa-client-0.9.5/sherpa_client/api/gazetteers/delete_gazetteers.py
--rw-r--r--   0        0        0     2343 2021-12-02 09:15:39.139671 sherpa-client-0.9.5/sherpa_client/api/gazetteers/export_gazetteer.py
--rw-r--r--   0        0        0     2731 2021-12-02 09:15:39.215670 sherpa-client-0.9.5/sherpa_client/api/gazetteers/export_gazetteers.py
--rw-r--r--   0        0        0     2531 2021-12-02 09:15:39.187671 sherpa-client-0.9.5/sherpa_client/api/gazetteers/get_gazetteer.py
--rw-r--r--   0        0        0     2499 2021-12-02 09:15:39.159671 sherpa-client-0.9.5/sherpa_client/api/gazetteers/get_gazetteers.py
--rw-r--r--   0        0        0     2535 2021-12-02 09:15:39.187671 sherpa-client-0.9.5/sherpa_client/api/gazetteers/patch_gazetteer.py
--rw-r--r--   0        0        0     2598 2021-12-02 09:15:39.191671 sherpa-client-0.9.5/sherpa_client/api/gazetteers/synchronize_gazetteer.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.655701 sherpa-client-0.9.5/sherpa_client/api/groups/__init__.py
--rw-r--r--   0        0        0     2266 2021-12-02 09:15:39.223671 sherpa-client-0.9.5/sherpa_client/api/groups/add_group.py
--rw-r--r--   0        0        0     2921 2021-12-02 09:15:39.263670 sherpa-client-0.9.5/sherpa_client/api/groups/delete_group.py
--rw-r--r--   0        0        0     2314 2021-12-02 09:15:39.243670 sherpa-client-0.9.5/sherpa_client/api/groups/get_group.py
--rw-r--r--   0        0        0     2192 2021-12-02 09:15:39.207671 sherpa-client-0.9.5/sherpa_client/api/groups/get_groups.py
--rw-r--r--   0        0        0     2263 2021-12-02 09:15:39.303670 sherpa-client-0.9.5/sherpa_client/api/groups/patch_group.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.639701 sherpa-client-0.9.5/sherpa_client/api/jobs/__init__.py
--rw-r--r--   0        0        0     2293 2021-12-02 09:15:39.327670 sherpa-client-0.9.5/sherpa_client/api/jobs/cancel_global_job.py
--rw-r--r--   0        0        0     2600 2021-12-02 09:15:39.319670 sherpa-client-0.9.5/sherpa_client/api/jobs/cancel_job.py
--rw-r--r--   0        0        0     2896 2021-12-02 09:15:39.399670 sherpa-client-0.9.5/sherpa_client/api/jobs/get_all_jobs.py
--rw-r--r--   0        0        0     2287 2021-12-02 09:15:39.371670 sherpa-client-0.9.5/sherpa_client/api/jobs/get_global_job.py
--rw-r--r--   0        0        0     2594 2021-12-02 09:15:39.335670 sherpa-client-0.9.5/sherpa_client/api/jobs/get_job.py
--rw-r--r--   0        0        0     3204 2021-12-02 09:15:39.383670 sherpa-client-0.9.5/sherpa_client/api/jobs/get_jobs.py
--rw-r--r--   0        0        0     3306 2021-12-02 09:15:39.387670 sherpa-client-0.9.5/sherpa_client/api/jobs/launch_dummy_job.py
--rw-r--r--   0        0        0     2616 2021-12-02 09:15:39.419670 sherpa-client-0.9.5/sherpa_client/api/jobs/wait_for_job.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.659701 sherpa-client-0.9.5/sherpa_client/api/labels/__init__.py
--rw-r--r--   0        0        0     2536 2021-12-02 09:15:39.383670 sherpa-client-0.9.5/sherpa_client/api/labels/create_label.py
--rw-r--r--   0        0        0     2687 2021-12-02 09:15:39.395670 sherpa-client-0.9.5/sherpa_client/api/labels/delete_label_by_name.py
--rw-r--r--   0        0        0     3067 2021-12-02 09:15:39.451670 sherpa-client-0.9.5/sherpa_client/api/labels/get_labels.py
--rw-r--r--   0        0        0     2808 2021-12-02 09:15:39.559669 sherpa-client-0.9.5/sherpa_client/api/labels/update_label.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.595701 sherpa-client-0.9.5/sherpa_client/api/lexicons/__init__.py
--rw-r--r--   0        0        0     2726 2021-12-02 09:15:39.463670 sherpa-client-0.9.5/sherpa_client/api/lexicons/create_lexicon.py
--rw-r--r--   0        0        0     2941 2021-12-02 09:15:39.555669 sherpa-client-0.9.5/sherpa_client/api/lexicons/create_term.py
--rw-r--r--   0        0        0     2621 2021-12-02 09:15:39.491670 sherpa-client-0.9.5/sherpa_client/api/lexicons/delete_lexicon_by_name.py
--rw-r--r--   0        0        0     3298 2021-12-02 09:15:39.563669 sherpa-client-0.9.5/sherpa_client/api/lexicons/get_lexicon.py
--rw-r--r--   0        0        0     3125 2021-12-02 09:15:39.551669 sherpa-client-0.9.5/sherpa_client/api/lexicons/get_lexicons.py
--rw-r--r--   0        0        0     3089 2021-12-02 09:15:39.563669 sherpa-client-0.9.5/sherpa_client/api/lexicons/launch_uploaded_terms_import.py
--rw-r--r--   0        0        0     6091 2021-12-02 09:15:39.851668 sherpa-client-0.9.5/sherpa_client/api/lexicons/search_terms.py
--rw-r--r--   0        0        0     2483 2021-12-02 09:15:39.547669 sherpa-client-0.9.5/sherpa_client/api/lexicons/update_lexicon.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.555702 sherpa-client-0.9.5/sherpa_client/api/metrics/__init__.py
--rw-r--r--   0        0        0     2751 2021-12-02 09:15:39.595669 sherpa-client-0.9.5/sherpa_client/api/metrics/get_annotation_metrics.py
--rw-r--r--   0        0        0     2733 2021-12-02 09:15:39.659669 sherpa-client-0.9.5/sherpa_client/api/metrics/get_categories_metrics.py
--rw-r--r--   0        0        0     2711 2021-12-02 09:15:39.619669 sherpa-client-0.9.5/sherpa_client/api/metrics/get_corpus_metrics.py
--rw-r--r--   0        0        0     2225 2021-12-02 09:15:39.591669 sherpa-client-0.9.5/sherpa_client/api/metrics/get_model_metrics.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.655701 sherpa-client-0.9.5/sherpa_client/api/models/__init__.py
--rw-r--r--   0        0        0     1430 2021-12-02 09:15:39.575669 sherpa-client-0.9.5/sherpa_client/api/models/delete_models.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.559702 sherpa-client-0.9.5/sherpa_client/api/plans/__init__.py
--rw-r--r--   0        0        0     2652 2021-12-02 09:15:39.695669 sherpa-client-0.9.5/sherpa_client/api/plans/compute_plan_label_hint.py
--rw-r--r--   0        0        0     2653 2021-12-02 09:15:39.687669 sherpa-client-0.9.5/sherpa_client/api/plans/create_plan.py
--rw-r--r--   0        0        0     2578 2021-12-02 09:15:39.759668 sherpa-client-0.9.5/sherpa_client/api/plans/delete_plan.py
--rw-r--r--   0        0        0     2579 2021-12-02 09:15:39.843668 sherpa-client-0.9.5/sherpa_client/api/plans/delete_plans.py
--rw-r--r--   0        0        0     2618 2021-12-02 09:15:39.715669 sherpa-client-0.9.5/sherpa_client/api/plans/get_plan.py
--rw-r--r--   0        0        0     2664 2021-12-02 09:15:39.695669 sherpa-client-0.9.5/sherpa_client/api/plans/get_plans.py
--rw-r--r--   0        0        0     2622 2021-12-02 09:15:39.723669 sherpa-client-0.9.5/sherpa_client/api/plans/patch_plan.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.611701 sherpa-client-0.9.5/sherpa_client/api/project_engines/__init__.py
--rw-r--r--   0        0        0     3453 2021-12-02 09:15:39.771669 sherpa-client-0.9.5/sherpa_client/api/project_engines/get_project_engine_parameters_schema.py
--rw-r--r--   0        0        0     2480 2021-12-02 09:15:39.751669 sherpa-client-0.9.5/sherpa_client/api/project_engines/get_project_engines.py
--rw-r--r--   0        0        0     4454 2021-12-02 09:15:39.887668 sherpa-client-0.9.5/sherpa_client/api/project_engines/get_project_services.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.615701 sherpa-client-0.9.5/sherpa_client/api/projects/__init__.py
--rw-r--r--   0        0        0     1694 2021-12-02 09:15:39.775668 sherpa-client-0.9.5/sherpa_client/api/projects/auto_discover_on_corpus.py
--rw-r--r--   0        0        0     2089 2021-12-02 09:15:39.815668 sherpa-client-0.9.5/sherpa_client/api/projects/compute_train_test_split.py
--rw-r--r--   0        0        0     2941 2021-12-02 09:15:39.887668 sherpa-client-0.9.5/sherpa_client/api/projects/create_project.py
--rw-r--r--   0        0        0     4578 2021-12-02 09:15:39.959668 sherpa-client-0.9.5/sherpa_client/api/projects/create_project_from_archive.py
--rw-r--r--   0        0        0     4301 2021-12-02 09:15:39.995668 sherpa-client-0.9.5/sherpa_client/api/projects/create_project_from_uploaded_archive.py
--rw-r--r--   0        0        0     1927 2021-12-02 09:15:39.831668 sherpa-client-0.9.5/sherpa_client/api/projects/create_tour_project.py
--rw-r--r--   0        0        0     2299 2021-12-02 09:15:39.891668 sherpa-client-0.9.5/sherpa_client/api/projects/delete_project.py
--rw-r--r--   0        0        0     2098 2021-12-02 09:15:39.899668 sherpa-client-0.9.5/sherpa_client/api/projects/delete_tour_project.py
--rw-r--r--   0        0        0     2545 2021-12-02 09:15:39.927668 sherpa-client-0.9.5/sherpa_client/api/projects/deploy_project.py
--rw-r--r--   0        0        0     2470 2021-12-02 09:15:39.919668 sherpa-client-0.9.5/sherpa_client/api/projects/export_dataset.py
--rw-r--r--   0        0        0     3124 2021-12-02 09:15:40.059667 sherpa-client-0.9.5/sherpa_client/api/projects/export_models.py
--rw-r--r--   0        0        0     2779 2021-12-02 09:15:39.999668 sherpa-client-0.9.5/sherpa_client/api/projects/export_project.py
--rw-r--r--   0        0        0     2079 2021-12-02 09:15:40.015668 sherpa-client-0.9.5/sherpa_client/api/projects/flush_indices.py
--rw-r--r--   0        0        0     1998 2021-12-02 09:15:39.955668 sherpa-client-0.9.5/sherpa_client/api/projects/get_app_state.py
--rw-r--r--   0        0        0     2201 2021-12-02 09:15:40.043667 sherpa-client-0.9.5/sherpa_client/api/projects/get_config.py
--rw-r--r--   0        0        0     2649 2021-12-02 09:15:40.027668 sherpa-client-0.9.5/sherpa_client/api/projects/get_metadata_definition.py
--rw-r--r--   0        0        0     3786 2021-12-02 09:15:40.115667 sherpa-client-0.9.5/sherpa_client/api/projects/get_project_info.py
--rw-r--r--   0        0        0     4644 2021-12-02 09:15:40.227667 sherpa-client-0.9.5/sherpa_client/api/projects/get_projects.py
--rw-r--r--   0        0        0     2241 2021-12-02 09:15:40.055667 sherpa-client-0.9.5/sherpa_client/api/projects/get_properties.py
--rw-r--r--   0        0        0     2927 2021-12-02 09:15:40.095667 sherpa-client-0.9.5/sherpa_client/api/projects/import_archive.py
--rw-r--r--   0        0        0     2916 2021-12-02 09:15:40.095667 sherpa-client-0.9.5/sherpa_client/api/projects/import_models.py
--rw-r--r--   0        0        0     3004 2021-12-02 09:15:40.107667 sherpa-client-0.9.5/sherpa_client/api/projects/import_uploaded_archive.py
--rw-r--r--   0        0        0     3000 2021-12-02 09:15:40.163667 sherpa-client-0.9.5/sherpa_client/api/projects/import_uploaded_models.py
--rw-r--r--   0        0        0     2714 2021-12-02 09:15:40.163667 sherpa-client-0.9.5/sherpa_client/api/projects/launch_project_reindexing.py
--rw-r--r--   0        0        0     2967 2021-12-02 09:15:40.179667 sherpa-client-0.9.5/sherpa_client/api/projects/launch_project_restoration_from_backup.py
--rw-r--r--   0        0        0     2677 2021-12-02 09:15:40.171667 sherpa-client-0.9.5/sherpa_client/api/projects/launch_project_restoration_from_image.py
--rw-r--r--   0        0        0     5107 2021-12-02 09:15:40.319666 sherpa-client-0.9.5/sherpa_client/api/projects/maybe_create_projects_and_import_models_from_archive.py
--rw-r--r--   0        0        0     2415 2021-12-02 09:15:40.227667 sherpa-client-0.9.5/sherpa_client/api/projects/reindex_projects.py
--rw-r--r--   0        0        0     2456 2021-12-02 09:15:40.303667 sherpa-client-0.9.5/sherpa_client/api/projects/undeploy_project.py
--rw-r--r--   0        0        0     1428 2021-12-02 09:15:40.231667 sherpa-client-0.9.5/sherpa_client/api/projects/update_config_options.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.651701 sherpa-client-0.9.5/sherpa_client/api/roles/__init__.py
--rw-r--r--   0        0        0     3191 2021-12-02 09:15:40.291667 sherpa-client-0.9.5/sherpa_client/api/roles/add_role.py
--rw-r--r--   0        0        0     2234 2021-12-02 09:15:40.243667 sherpa-client-0.9.5/sherpa_client/api/roles/delete_role.py
--rw-r--r--   0        0        0     1845 2021-12-02 09:15:40.231667 sherpa-client-0.9.5/sherpa_client/api/roles/get_permissions.py
--rw-r--r--   0        0        0     2274 2021-12-02 09:15:40.295667 sherpa-client-0.9.5/sherpa_client/api/roles/get_role.py
--rw-r--r--   0        0        0     2178 2021-12-02 09:15:40.283667 sherpa-client-0.9.5/sherpa_client/api/roles/get_roles.py
--rw-r--r--   0        0        0     2232 2021-12-02 09:15:40.307667 sherpa-client-0.9.5/sherpa_client/api/roles/update_role.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.607701 sherpa-client-0.9.5/sherpa_client/api/segments/__init__.py
--rw-r--r--   0        0        0     7194 2021-12-02 09:15:40.699665 sherpa-client-0.9.5/sherpa_client/api/segments/find_similar_segments.py
--rw-r--r--   0        0        0     6738 2021-12-02 09:15:40.595666 sherpa-client-0.9.5/sherpa_client/api/segments/get_segment_context.py
--rw-r--r--   0        0        0     6559 2021-12-02 09:15:40.623665 sherpa-client-0.9.5/sherpa_client/api/segments/search_segments.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.571701 sherpa-client-0.9.5/sherpa_client/api/services/__init__.py
--rw-r--r--   0        0        0     3529 2021-12-02 09:15:40.431666 sherpa-client-0.9.5/sherpa_client/api/services/get_engine_parameters_schema.py
--rw-r--r--   0        0        0     7071 2021-12-02 09:15:40.883664 sherpa-client-0.9.5/sherpa_client/api/services/get_services.py
--rw-r--r--   0        0        0     6778 2021-12-02 09:15:40.851665 sherpa-client-0.9.5/sherpa_client/api/services/get_services_distinct_values.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.591701 sherpa-client-0.9.5/sherpa_client/api/shares/__init__.py
--rw-r--r--   0        0        0     1879 2021-12-02 09:15:40.399666 sherpa-client-0.9.5/sherpa_client/api/shares/change_project_ownership.py
--rw-r--r--   0        0        0     1610 2021-12-02 09:15:40.379666 sherpa-client-0.9.5/sherpa_client/api/shares/delete_share_with_group.py
--rw-r--r--   0        0        0     1591 2021-12-02 09:15:40.399666 sherpa-client-0.9.5/sherpa_client/api/shares/delete_share_with_user.py
--rw-r--r--   0        0        0     2550 2021-12-02 09:15:40.487666 sherpa-client-0.9.5/sherpa_client/api/shares/get_group_shares.py
--rw-r--r--   0        0        0     2549 2021-12-02 09:15:40.439666 sherpa-client-0.9.5/sherpa_client/api/shares/get_user_shares.py
--rw-r--r--   0        0        0     2096 2021-12-02 09:15:40.427666 sherpa-client-0.9.5/sherpa_client/api/shares/share_with_group.py
--rw-r--r--   0        0        0     1980 2021-12-02 09:15:40.491666 sherpa-client-0.9.5/sherpa_client/api/shares/share_with_user.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.563701 sherpa-client-0.9.5/sherpa_client/api/suggesters/__init__.py
--rw-r--r--   0        0        0     2657 2021-12-02 09:15:40.535666 sherpa-client-0.9.5/sherpa_client/api/suggesters/compute_suggester_label_hint.py
--rw-r--r--   0        0        0     2586 2021-12-02 09:15:40.715665 sherpa-client-0.9.5/sherpa_client/api/suggesters/create_suggester.py
--rw-r--r--   0        0        0     2583 2021-12-02 09:15:40.559666 sherpa-client-0.9.5/sherpa_client/api/suggesters/delete_suggester.py
--rw-r--r--   0        0        0     2584 2021-12-02 09:15:40.583666 sherpa-client-0.9.5/sherpa_client/api/suggesters/delete_suggesters.py
--rw-r--r--   0        0        0     2531 2021-12-02 09:15:40.599665 sherpa-client-0.9.5/sherpa_client/api/suggesters/get_suggester.py
--rw-r--r--   0        0        0     2499 2021-12-02 09:15:40.623665 sherpa-client-0.9.5/sherpa_client/api/suggesters/get_suggesters.py
--rw-r--r--   0        0        0     2535 2021-12-02 09:15:40.659665 sherpa-client-0.9.5/sherpa_client/api/suggesters/patch_suggester.py
--rw-r--r--   0        0        0     2500 2021-12-02 09:15:40.767665 sherpa-client-0.9.5/sherpa_client/api/suggesters/start_suggester.py
--rw-r--r--   0        0        0     1551 2021-12-02 09:15:40.659665 sherpa-client-0.9.5/sherpa_client/api/suggesters/stop_suggester.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.567701 sherpa-client-0.9.5/sherpa_client/api/suggestions/__init__.py
--rw-r--r--   0        0        0     2242 2021-12-02 09:15:40.719665 sherpa-client-0.9.5/sherpa_client/api/suggestions/clear_suggestions.py
--rw-r--r--   0        0        0     2640 2021-12-02 09:15:40.743665 sherpa-client-0.9.5/sherpa_client/api/suggestions/delete_suggestion.py
--rw-r--r--   0        0        0     4581 2021-12-02 09:15:40.875665 sherpa-client-0.9.5/sherpa_client/api/suggestions/get_suggestions.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.555702 sherpa-client-0.9.5/sherpa_client/api/uploads/__init__.py
--rw-r--r--   0        0        0     2253 2021-12-02 09:15:40.763665 sherpa-client-0.9.5/sherpa_client/api/uploads/get_uploaded_file_info.py
--rw-r--r--   0        0        0     3621 2021-12-02 09:15:40.815665 sherpa-client-0.9.5/sherpa_client/api/uploads/upload_files.py
--rw-r--r--   0        0        0        0 2021-12-02 09:15:30.599701 sherpa-client-0.9.5/sherpa_client/api/users/__init__.py
--rw-r--r--   0        0        0     2830 2021-12-02 09:15:40.835665 sherpa-client-0.9.5/sherpa_client/api/users/add_user.py
--rw-r--r--   0        0        0     2234 2021-12-02 09:15:40.775665 sherpa-client-0.9.5/sherpa_client/api/users/delete_user.py
--rw-r--r--   0        0        0     3288 2021-12-02 09:15:40.899664 sherpa-client-0.9.5/sherpa_client/api/users/get_user.py
--rw-r--r--   0        0        0     3245 2021-12-02 09:15:40.939664 sherpa-client-0.9.5/sherpa_client/api/users/get_users.py
--rw-r--r--   0        0        0     2232 2021-12-02 09:15:40.883664 sherpa-client-0.9.5/sherpa_client/api/users/update_permissions.py
--rw-r--r--   0        0        0     2240 2021-12-02 09:15:40.927664 sherpa-client-0.9.5/sherpa_client/api/users/update_profile.py
--rw-r--r--   0        0        0     2697 2021-12-02 12:15:29.597648 sherpa-client-0.9.5/sherpa_client/client.py
--rw-r--r--   0        0        0     8820 2021-12-02 09:15:37.867675 sherpa-client-0.9.5/sherpa_client/models/__init__.py
--rw-r--r--   0        0        0      580 2021-12-02 09:15:40.819665 sherpa-client-0.9.5/sherpa_client/models/ack.py
--rw-r--r--   0        0        0     1133 2021-12-02 09:15:40.911664 sherpa-client-0.9.5/sherpa_client/models/aggregation.py
--rw-r--r--   0        0        0     2232 2021-12-02 09:15:40.959664 sherpa-client-0.9.5/sherpa_client/models/annotate_binary_form.py
--rw-r--r--   0        0        0     2315 2021-12-02 09:15:40.967664 sherpa-client-0.9.5/sherpa_client/models/annotate_binary_with_plan_ref_multipart_data.py
--rw-r--r--   0        0        0     2505 2021-12-02 09:15:40.991664 sherpa-client-0.9.5/sherpa_client/models/annotate_documents_with_many.py
--rw-r--r--   0        0        0     2348 2021-12-02 09:15:40.995664 sherpa-client-0.9.5/sherpa_client/models/annotate_format_binary_with_plan_ref_multipart_data.py
--rw-r--r--   0        0        0     2038 2021-12-02 09:15:40.971664 sherpa-client-0.9.5/sherpa_client/models/annotate_text_with_many.py
--rw-r--r--   0        0        0     3199 2021-12-02 09:15:41.083664 sherpa-client-0.9.5/sherpa_client/models/annotated_doc_annotation.py
--rw-r--r--   0        0        0     1279 2021-12-02 09:15:40.951664 sherpa-client-0.9.5/sherpa_client/models/annotated_doc_annotation_properties.py
--rw-r--r--   0        0        0     2124 2021-12-02 09:15:40.999664 sherpa-client-0.9.5/sherpa_client/models/annotated_doc_category.py
--rw-r--r--   0        0        0     1269 2021-12-02 09:15:40.971664 sherpa-client-0.9.5/sherpa_client/models/annotated_doc_category_properties.py
--rw-r--r--   0        0        0     4262 2021-12-02 09:15:41.131664 sherpa-client-0.9.5/sherpa_client/models/annotated_document.py
--rw-r--r--   0        0        0     1237 2021-12-02 09:15:41.007664 sherpa-client-0.9.5/sherpa_client/models/annotated_document_metadata.py
--rw-r--r--   0        0        0     1911 2021-12-02 09:15:41.147664 sherpa-client-0.9.5/sherpa_client/models/annotation.py
--rw-r--r--   0        0        0     1498 2021-12-02 09:15:41.031664 sherpa-client-0.9.5/sherpa_client/models/annotation_facets.py
--rw-r--r--   0        0        0      716 2021-12-02 09:15:40.999664 sherpa-client-0.9.5/sherpa_client/models/annotation_id.py
--rw-r--r--   0        0        0     2513 2021-12-02 09:15:41.063664 sherpa-client-0.9.5/sherpa_client/models/annotation_metrics.py
--rw-r--r--   0        0        0     3107 2021-12-02 09:15:41.131664 sherpa-client-0.9.5/sherpa_client/models/annotation_plan.py
--rw-r--r--   0        0        0      149 2021-12-02 09:15:40.991664 sherpa-client-0.9.5/sherpa_client/models/annotation_status.py
--rw-r--r--   0        0        0     2064 2021-12-02 09:15:41.103664 sherpa-client-0.9.5/sherpa_client/models/annotation_term.py
--rw-r--r--   0        0        0     1237 2021-12-02 09:15:41.127664 sherpa-client-0.9.5/sherpa_client/models/annotation_term_properties.py
--rw-r--r--   0        0        0     1340 2021-12-02 09:15:41.079664 sherpa-client-0.9.5/sherpa_client/models/annotator.py
--rw-r--r--   0        0        0     2007 2021-12-02 09:15:41.095664 sherpa-client-0.9.5/sherpa_client/models/annotator_multimap.py
--rw-r--r--   0        0        0     1044 2021-12-02 12:30:35.358108 sherpa-client-0.9.5/sherpa_client/models/bearer_token.py
--rw-r--r--   0        0        0      767 2021-12-02 09:15:41.059664 sherpa-client-0.9.5/sherpa_client/models/bucket.py
--rw-r--r--   0        0        0     1029 2021-12-02 09:15:41.087664 sherpa-client-0.9.5/sherpa_client/models/categories_facets.py
--rw-r--r--   0        0        0     1726 2021-12-02 09:15:41.147664 sherpa-client-0.9.5/sherpa_client/models/category.py
--rw-r--r--   0        0        0      681 2021-12-02 09:15:41.111664 sherpa-client-0.9.5/sherpa_client/models/category_id.py
--rw-r--r--   0        0        0     1679 2021-12-02 09:15:41.135664 sherpa-client-0.9.5/sherpa_client/models/category_metrics.py
--rw-r--r--   0        0        0      147 2021-12-02 09:15:41.087664 sherpa-client-0.9.5/sherpa_client/models/category_status.py
--rw-r--r--   0        0        0      785 2021-12-02 09:15:41.127664 sherpa-client-0.9.5/sherpa_client/models/classification_config.py
--rw-r--r--   0        0        0      874 2021-12-02 09:15:41.147664 sherpa-client-0.9.5/sherpa_client/models/classification_options.py
--rw-r--r--   0        0        0     2074 2021-12-02 09:15:41.211663 sherpa-client-0.9.5/sherpa_client/models/config_patch_options.py
--rw-r--r--   0        0        0     2164 2021-12-02 09:15:41.239663 sherpa-client-0.9.5/sherpa_client/models/convert_annotation_plan.py
--rw-r--r--   0        0        0     2436 2021-12-02 09:15:41.215663 sherpa-client-0.9.5/sherpa_client/models/convert_format_annotation_plan.py
--rw-r--r--   0        0        0     1322 2021-12-02 09:15:41.195663 sherpa-client-0.9.5/sherpa_client/models/converter.py
--rw-r--r--   0        0        0     1217 2021-12-02 09:15:41.223663 sherpa-client-0.9.5/sherpa_client/models/converter_parameters.py
--rw-r--r--   0        0        0     1430 2021-12-02 09:15:41.219663 sherpa-client-0.9.5/sherpa_client/models/corpus_metrics.py
--rw-r--r--   0        0        0     1219 2021-12-02 09:15:41.199663 sherpa-client-0.9.5/sherpa_client/models/create_lexicon_response_200.py
--rw-r--r--   0        0        0     2307 2021-12-02 09:15:41.283663 sherpa-client-0.9.5/sherpa_client/models/create_project_from_archive_multipart_data.py
--rw-r--r--   0        0        0     1204 2021-12-02 09:15:41.203663 sherpa-client-0.9.5/sherpa_client/models/create_term_response_200.py
--rw-r--r--   0        0        0      828 2021-12-02 09:15:41.195663 sherpa-client-0.9.5/sherpa_client/models/created_by_count.py
--rw-r--r--   0        0        0      796 2021-12-02 09:15:41.199663 sherpa-client-0.9.5/sherpa_client/models/credentials.py
--rw-r--r--   0        0        0      964 2021-12-02 09:15:41.207663 sherpa-client-0.9.5/sherpa_client/models/delete_group_result.py
--rw-r--r--   0        0        0     1392 2021-12-02 09:15:41.271663 sherpa-client-0.9.5/sherpa_client/models/delete_response.py
--rw-r--r--   0        0        0     2727 2021-12-02 09:15:41.379663 sherpa-client-0.9.5/sherpa_client/models/doc_annotation.py
--rw-r--r--   0        0        0      152 2021-12-02 09:15:41.207663 sherpa-client-0.9.5/sherpa_client/models/doc_annotation_status.py
--rw-r--r--   0        0        0     2469 2021-12-02 09:15:41.359663 sherpa-client-0.9.5/sherpa_client/models/doc_category.py
--rw-r--r--   0        0        0      150 2021-12-02 09:15:41.215663 sherpa-client-0.9.5/sherpa_client/models/doc_category_status.py
--rw-r--r--   0        0        0      753 2021-12-02 09:15:41.259663 sherpa-client-0.9.5/sherpa_client/models/doc_sentence.py
--rw-r--r--   0        0        0     4755 2021-12-02 09:15:41.455663 sherpa-client-0.9.5/sherpa_client/models/document.py
--rw-r--r--   0        0        0     1191 2021-12-02 09:15:41.279663 sherpa-client-0.9.5/sherpa_client/models/document_facets.py
--rw-r--r--   0        0        0      981 2021-12-02 09:15:41.275663 sherpa-client-0.9.5/sherpa_client/models/document_hit.py
--rw-r--r--   0        0        0     2313 2021-12-02 09:15:41.423663 sherpa-client-0.9.5/sherpa_client/models/document_hits.py
--rw-r--r--   0        0        0     1189 2021-12-02 09:15:41.331663 sherpa-client-0.9.5/sherpa_client/models/document_metadata.py
--rw-r--r--   0        0        0      757 2021-12-02 09:15:41.299663 sherpa-client-0.9.5/sherpa_client/models/engine_config.py
--rw-r--r--   0        0        0     2126 2021-12-02 09:15:41.367663 sherpa-client-0.9.5/sherpa_client/models/engine_config_import_summary.py
--rw-r--r--   0        0        0      627 2021-12-02 09:15:41.311663 sherpa-client-0.9.5/sherpa_client/models/engine_name.py
--rw-r--r--   0        0        0     2916 2021-12-02 09:15:41.443663 sherpa-client-0.9.5/sherpa_client/models/experiment.py
--rw-r--r--   0        0        0     1193 2021-12-02 09:15:41.347663 sherpa-client-0.9.5/sherpa_client/models/experiment_parameters.py
--rw-r--r--   0        0        0     1651 2021-12-02 09:15:41.371663 sherpa-client-0.9.5/sherpa_client/models/experiment_patch.py
--rw-r--r--   0        0        0     1221 2021-12-02 09:15:41.367663 sherpa-client-0.9.5/sherpa_client/models/experiment_patch_parameters.py
--rw-r--r--   0        0        0     2255 2021-12-02 09:15:41.487662 sherpa-client-0.9.5/sherpa_client/models/format_binary_form.py
--rw-r--r--   0        0        0     2743 2021-12-02 09:15:41.455663 sherpa-client-0.9.5/sherpa_client/models/format_documents_with_many.py
--rw-r--r--   0        0        0     2276 2021-12-02 09:15:41.475662 sherpa-client-0.9.5/sherpa_client/models/format_text_with_many.py
--rw-r--r--   0        0        0     1322 2021-12-02 09:15:41.423663 sherpa-client-0.9.5/sherpa_client/models/formatter.py
--rw-r--r--   0        0        0     1217 2021-12-02 09:15:41.443663 sherpa-client-0.9.5/sherpa_client/models/formatter_parameters.py
--rw-r--r--   0        0        0     1962 2021-12-02 09:15:41.511662 sherpa-client-0.9.5/sherpa_client/models/gazetteer.py
--rw-r--r--   0        0        0     1188 2021-12-02 09:15:41.439663 sherpa-client-0.9.5/sherpa_client/models/gazetteer_parameters.py
--rw-r--r--   0        0        0     1412 2021-12-02 09:15:41.451662 sherpa-client-0.9.5/sherpa_client/models/gazetteer_patch.py
--rw-r--r--   0        0        0     1216 2021-12-02 09:15:41.463662 sherpa-client-0.9.5/sherpa_client/models/gazetteer_patch_parameters.py
--rw-r--r--   0        0        0      713 2021-12-02 09:15:41.463662 sherpa-client-0.9.5/sherpa_client/models/generated_label_hint.py
--rw-r--r--   0        0        0     1212 2021-12-02 09:15:41.491662 sherpa-client-0.9.5/sherpa_client/models/get_app_state_response_200.py
--rw-r--r--   0        0        0     1285 2021-12-02 09:15:41.511662 sherpa-client-0.9.5/sherpa_client/models/get_engine_parameters_schema_response_200.py
--rw-r--r--   0        0        0     1323 2021-12-02 09:15:41.511662 sherpa-client-0.9.5/sherpa_client/models/get_project_engine_parameters_schema_response_200.py
--rw-r--r--   0        0        0      217 2021-12-02 09:15:41.463662 sherpa-client-0.9.5/sherpa_client/models/get_segment_context_context_output.py
--rw-r--r--   0        0        0     1224 2021-12-02 09:15:41.519662 sherpa-client-0.9.5/sherpa_client/models/get_suggestions_response_200.py
--rw-r--r--   0        0        0     2405 2021-12-02 09:15:41.599662 sherpa-client-0.9.5/sherpa_client/models/group_desc.py
--rw-r--r--   0        0        0      623 2021-12-02 09:15:41.511662 sherpa-client-0.9.5/sherpa_client/models/group_name.py
--rw-r--r--   0        0        0     1384 2021-12-02 09:15:41.639662 sherpa-client-0.9.5/sherpa_client/models/group_patch.py
--rw-r--r--   0        0        0     1057 2021-12-02 09:15:41.527662 sherpa-client-0.9.5/sherpa_client/models/group_share.py
--rw-r--r--   0        0        0     4418 2021-12-02 09:15:41.751661 sherpa-client-0.9.5/sherpa_client/models/http_service_metadata.py
--rw-r--r--   0        0        0     1244 2021-12-02 09:15:41.535662 sherpa-client-0.9.5/sherpa_client/models/http_service_metadata_operations.py
--rw-r--r--   0        0        0     1401 2021-12-02 09:15:41.583662 sherpa-client-0.9.5/sherpa_client/models/http_service_record.py
--rw-r--r--   0        0        0     2246 2021-12-02 09:15:41.647662 sherpa-client-0.9.5/sherpa_client/models/import_archive_multipart_data.py
--rw-r--r--   0        0        0     2241 2021-12-02 09:15:41.643662 sherpa-client-0.9.5/sherpa_client/models/import_models_multipart_data.py
--rw-r--r--   0        0        0     4152 2021-12-02 09:15:41.767661 sherpa-client-0.9.5/sherpa_client/models/input_document.py
--rw-r--r--   0        0        0     1217 2021-12-02 09:15:41.579662 sherpa-client-0.9.5/sherpa_client/models/input_document_metadata.py
--rw-r--r--   0        0        0      636 2021-12-02 09:15:41.559662 sherpa-client-0.9.5/sherpa_client/models/input_label.py
--rw-r--r--   0        0        0      452 2021-12-02 09:15:41.547662 sherpa-client-0.9.5/sherpa_client/models/job_status.py
--rw-r--r--   0        0        0      444 2021-12-02 09:15:41.563662 sherpa-client-0.9.5/sherpa_client/models/job_type.py
--rw-r--r--   0        0        0     1356 2021-12-02 09:15:41.619662 sherpa-client-0.9.5/sherpa_client/models/label.py
--rw-r--r--   0        0        0      742 2021-12-02 09:15:41.599662 sherpa-client-0.9.5/sherpa_client/models/label_count.py
--rw-r--r--   0        0        0     1162 2021-12-02 09:15:41.631662 sherpa-client-0.9.5/sherpa_client/models/label_update.py
--rw-r--r--   0        0        0     2284 2021-12-02 09:15:41.699662 sherpa-client-0.9.5/sherpa_client/models/launch_document_import_multipart_data.py
--rw-r--r--   0        0        0      323 2021-12-02 09:15:41.595662 sherpa-client-0.9.5/sherpa_client/models/launch_document_import_segmentation_policy.py
--rw-r--r--   0        0        0     2360 2021-12-02 09:15:41.711662 sherpa-client-0.9.5/sherpa_client/models/launch_project_restoration_from_backup_multipart_data.py
--rw-r--r--   0        0        0      331 2021-12-02 09:15:41.607662 sherpa-client-0.9.5/sherpa_client/models/launch_uploaded_document_import_segmentation_policy.py
--rw-r--r--   0        0        0     2404 2021-12-02 09:15:41.731661 sherpa-client-0.9.5/sherpa_client/models/lexicon.py
--rw-r--r--   0        0        0      921 2021-12-02 09:15:41.659662 sherpa-client-0.9.5/sherpa_client/models/lexicon_update.py
--rw-r--r--   0        0        0     2424 2021-12-02 09:15:41.743661 sherpa-client-0.9.5/sherpa_client/models/maybe_create_projects_and_import_models_from_archive_multipart_data.py
--rw-r--r--   0        0        0     1034 2021-12-02 09:15:41.719662 sherpa-client-0.9.5/sherpa_client/models/metadata_count.py
--rw-r--r--   0        0        0     1132 2021-12-02 09:15:41.691662 sherpa-client-0.9.5/sherpa_client/models/metadata_definition.py
--rw-r--r--   0        0        0     1461 2021-12-02 09:15:41.703662 sherpa-client-0.9.5/sherpa_client/models/metadata_definition_entry.py
--rw-r--r--   0        0        0     2452 2021-12-02 09:15:41.787661 sherpa-client-0.9.5/sherpa_client/models/model_metrics.py
--rw-r--r--   0        0        0     1191 2021-12-02 09:15:41.715662 sherpa-client-0.9.5/sherpa_client/models/model_metrics_options.py
--rw-r--r--   0        0        0     2038 2021-12-02 09:15:41.783661 sherpa-client-0.9.5/sherpa_client/models/models_metrics.py
--rw-r--r--   0        0        0     2351 2021-12-02 09:15:41.823661 sherpa-client-0.9.5/sherpa_client/models/named_annotation_plan.py
--rw-r--r--   0        0        0     1101 2021-12-02 09:15:41.767661 sherpa-client-0.9.5/sherpa_client/models/new_experiment.py
--rw-r--r--   0        0        0     1211 2021-12-02 09:15:41.791661 sherpa-client-0.9.5/sherpa_client/models/new_experiment_parameters.py
--rw-r--r--   0        0        0     1093 2021-12-02 09:15:41.771661 sherpa-client-0.9.5/sherpa_client/models/new_gazetteer.py
--rw-r--r--   0        0        0     1206 2021-12-02 09:15:41.783661 sherpa-client-0.9.5/sherpa_client/models/new_gazetteer_parameters.py
--rw-r--r--   0        0        0     1361 2021-12-02 09:15:41.815661 sherpa-client-0.9.5/sherpa_client/models/new_group_desc.py
--rw-r--r--   0        0        0      964 2021-12-02 09:15:41.783661 sherpa-client-0.9.5/sherpa_client/models/new_named_annotation_plan.py
--rw-r--r--   0        0        0      844 2021-12-02 09:15:41.795661 sherpa-client-0.9.5/sherpa_client/models/new_role.py
--rw-r--r--   0        0        0     1093 2021-12-02 09:15:41.811661 sherpa-client-0.9.5/sherpa_client/models/new_suggester.py
--rw-r--r--   0        0        0     1206 2021-12-02 09:15:41.883661 sherpa-client-0.9.5/sherpa_client/models/new_suggester_parameters.py
--rw-r--r--   0        0        0     1184 2021-12-02 09:15:41.839661 sherpa-client-0.9.5/sherpa_client/models/new_user.py
--rw-r--r--   0        0        0      968 2021-12-02 09:15:41.831661 sherpa-client-0.9.5/sherpa_client/models/operation_count.py
--rw-r--r--   0        0        0     1355 2021-12-02 09:15:41.867661 sherpa-client-0.9.5/sherpa_client/models/partial_label.py
--rw-r--r--   0        0        0     1081 2021-12-02 09:15:41.851661 sherpa-client-0.9.5/sherpa_client/models/partial_lexicon.py
--rw-r--r--   0        0        0     1571 2021-12-02 09:15:41.879661 sherpa-client-0.9.5/sherpa_client/models/plan_patch.py
--rw-r--r--   0        0        0     6435 2021-12-02 09:15:42.163660 sherpa-client-0.9.5/sherpa_client/models/project_bean.py
--rw-r--r--   0        0        0     3338 2021-12-02 09:15:42.011660 sherpa-client-0.9.5/sherpa_client/models/project_config_creation.py
--rw-r--r--   0        0        0     1254 2021-12-02 09:15:41.863661 sherpa-client-0.9.5/sherpa_client/models/project_config_creation_properties.py
--rw-r--r--   0        0        0      722 2021-12-02 09:15:41.855661 sherpa-client-0.9.5/sherpa_client/models/project_property.py
--rw-r--r--   0        0        0     1536 2021-12-02 09:15:41.919661 sherpa-client-0.9.5/sherpa_client/models/project_status.py
--rw-r--r--   0        0        0     1349 2021-12-02 09:15:41.911661 sherpa-client-0.9.5/sherpa_client/models/quality_figures.py
--rw-r--r--   0        0        0      446 2021-12-02 09:15:41.859661 sherpa-client-0.9.5/sherpa_client/models/relation.py
--rw-r--r--   0        0        0     3375 2021-12-02 09:15:42.055660 sherpa-client-0.9.5/sherpa_client/models/report.py
--rw-r--r--   0        0        0     1550 2021-12-02 09:15:41.935661 sherpa-client-0.9.5/sherpa_client/models/report_classes.py
--rw-r--r--   0        0        0      195 2021-12-02 09:15:41.871661 sherpa-client-0.9.5/sherpa_client/models/request_jwt_token_project_access_mode.py
--rw-r--r--   0        0        0     2675 2021-12-02 09:15:42.043660 sherpa-client-0.9.5/sherpa_client/models/role_desc.py
--rw-r--r--   0        0        0     1113 2021-12-02 09:15:41.943661 sherpa-client-0.9.5/sherpa_client/models/role_update.py
--rw-r--r--   0        0        0      905 2021-12-02 09:15:41.919661 sherpa-client-0.9.5/sherpa_client/models/search_total.py
--rw-r--r--   0        0        0      154 2021-12-02 09:15:41.879661 sherpa-client-0.9.5/sherpa_client/models/search_total_relation.py
--rw-r--r--   0        0        0     3965 2021-12-02 09:15:42.087660 sherpa-client-0.9.5/sherpa_client/models/segment.py
--rw-r--r--   0        0        0     1910 2021-12-02 09:15:42.039660 sherpa-client-0.9.5/sherpa_client/models/segment_context.py
--rw-r--r--   0        0        0      944 2021-12-02 09:15:41.955661 sherpa-client-0.9.5/sherpa_client/models/segment_contexts.py
--rw-r--r--   0        0        0      964 2021-12-02 09:15:41.971661 sherpa-client-0.9.5/sherpa_client/models/segment_hit.py
--rw-r--r--   0        0        0     2305 2021-12-02 09:15:42.039660 sherpa-client-0.9.5/sherpa_client/models/segment_hits.py
--rw-r--r--   0        0        0     1168 2021-12-02 09:15:42.003661 sherpa-client-0.9.5/sherpa_client/models/segment_metadata.py
--rw-r--r--   0        0        0      756 2021-12-02 09:15:41.991660 sherpa-client-0.9.5/sherpa_client/models/share_mode.py
--rw-r--r--   0        0        0     3251 2021-12-02 09:15:42.107660 sherpa-client-0.9.5/sherpa_client/models/sherpa_job_bean.py
--rw-r--r--   0        0        0      248 2021-12-02 09:15:41.971661 sherpa-client-0.9.5/sherpa_client/models/sherpa_job_bean_status.py
--rw-r--r--   0        0        0      642 2021-12-02 09:15:41.999661 sherpa-client-0.9.5/sherpa_client/models/sherpa_job_bean_type.py
--rw-r--r--   0        0        0      883 2021-12-02 09:15:42.027660 sherpa-client-0.9.5/sherpa_client/models/simple_metadata.py
--rw-r--r--   0        0        0     2111 2021-12-02 09:15:42.123660 sherpa-client-0.9.5/sherpa_client/models/suggester.py
--rw-r--r--   0        0        0     1188 2021-12-02 09:15:42.063660 sherpa-client-0.9.5/sherpa_client/models/suggester_parameters.py
--rw-r--r--   0        0        0     1412 2021-12-02 09:15:42.091660 sherpa-client-0.9.5/sherpa_client/models/suggester_patch.py
--rw-r--r--   0        0        0     1216 2021-12-02 09:15:42.083660 sherpa-client-0.9.5/sherpa_client/models/suggester_patch_parameters.py
--rw-r--r--   0        0        0     1498 2021-12-02 09:15:42.111660 sherpa-client-0.9.5/sherpa_client/models/suggestion_facets.py
--rw-r--r--   0        0        0      655 2021-12-02 09:15:42.079660 sherpa-client-0.9.5/sherpa_client/models/term.py
--rw-r--r--   0        0        0      837 2021-12-02 09:15:42.095660 sherpa-client-0.9.5/sherpa_client/models/term_hit.py
--rw-r--r--   0        0        0     1151 2021-12-02 09:15:42.135660 sherpa-client-0.9.5/sherpa_client/models/term_hit_term.py
--rw-r--r--   0        0        0     1444 2021-12-02 09:15:42.135660 sherpa-client-0.9.5/sherpa_client/models/term_hits.py
--rw-r--r--   0        0        0     1259 2021-12-02 09:15:42.135660 sherpa-client-0.9.5/sherpa_client/models/term_import.py
--rw-r--r--   0        0        0     1004 2021-12-02 09:15:42.135660 sherpa-client-0.9.5/sherpa_client/models/term_importer_spec.py
--rw-r--r--   0        0        0     1229 2021-12-02 09:15:42.151660 sherpa-client-0.9.5/sherpa_client/models/term_importer_spec_parameters.py
--rw-r--r--   0        0        0      738 2021-12-02 09:15:42.163660 sherpa-client-0.9.5/sherpa_client/models/text_count.py
--rw-r--r--   0        0        0     2236 2021-12-02 09:15:42.223660 sherpa-client-0.9.5/sherpa_client/models/upload_files_multipart_data.py
--rw-r--r--   0        0        0     1083 2021-12-02 09:15:42.179660 sherpa-client-0.9.5/sherpa_client/models/uploaded_file.py
--rw-r--r--   0        0        0      635 2021-12-02 09:15:42.147660 sherpa-client-0.9.5/sherpa_client/models/uploaded_file_info.py
--rw-r--r--   0        0        0     1280 2021-12-02 09:15:42.211660 sherpa-client-0.9.5/sherpa_client/models/user_permissions_update.py
--rw-r--r--   0        0        0     1029 2021-12-02 09:15:42.187660 sherpa-client-0.9.5/sherpa_client/models/user_profile_update.py
--rw-r--r--   0        0        0     2724 2021-12-02 09:15:42.271659 sherpa-client-0.9.5/sherpa_client/models/user_response.py
--rw-r--r--   0        0        0     2563 2021-12-02 09:15:42.255660 sherpa-client-0.9.5/sherpa_client/models/with_annotator.py
--rw-r--r--   0        0        0     1206 2021-12-02 09:15:42.207660 sherpa-client-0.9.5/sherpa_client/models/with_annotator_condition.py
--rw-r--r--   0        0        0     1211 2021-12-02 09:15:42.199660 sherpa-client-0.9.5/sherpa_client/models/with_annotator_parameters.py
--rw-r--r--   0        0        0     2296 2021-12-02 09:15:42.259660 sherpa-client-0.9.5/sherpa_client/models/with_processor.py
--rw-r--r--   0        0        0     1206 2021-12-02 09:15:42.223660 sherpa-client-0.9.5/sherpa_client/models/with_processor_condition.py
--rw-r--r--   0        0        0     1211 2021-12-02 09:15:42.239660 sherpa-client-0.9.5/sherpa_client/models/with_processor_parameters.py
--rw-r--r--   0        0        0       25 2021-12-02 09:15:30.383702 sherpa-client-0.9.5/sherpa_client/py.typed
--rw-r--r--   0        0        0     4297 2021-12-02 12:57:22.895589 sherpa-client-0.9.5/sherpa_client/types.py
--rw-r--r--   0        0        0     5222 2021-12-02 12:58:03.931944 sherpa-client-0.9.5/setup.py
--rw-r--r--   0        0        0     4139 2021-12-02 12:58:03.932260 sherpa-client-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-12-02 10:16:57.780981 sherpa-client-0.9.6/LICENSE
+-rw-r--r--   0        0        0     3606 2021-12-02 09:15:30.387702 sherpa-client-0.9.6/README.md
+-rw-r--r--   0        0        0      825 2021-12-02 13:41:50.469601 sherpa-client-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0      112 2021-12-02 09:15:38.135674 sherpa-client-0.9.6/sherpa_client/__init__.py
+-rw-r--r--   0        0        0       47 2021-12-02 09:15:38.131674 sherpa-client-0.9.6/sherpa_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.579702 sherpa-client-0.9.6/sherpa_client/api/annotate/__init__.py
+-rw-r--r--   0        0        0     4860 2021-12-02 09:15:38.363674 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_binary.py
+-rw-r--r--   0        0        0     5574 2021-12-02 09:15:38.383674 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_binary_with_plan_ref.py
+-rw-r--r--   0        0        0     3581 2021-12-02 09:15:38.323674 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_corpus_with.py
+-rw-r--r--   0        0        0     5581 2021-12-02 09:15:38.395673 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_documents_with.py
+-rw-r--r--   0        0        0     4817 2021-12-02 09:15:38.363674 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_documents_with_many.py
+-rw-r--r--   0        0        0     3910 2021-12-02 09:15:38.319674 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_binary.py
+-rw-r--r--   0        0        0     4681 2021-12-02 09:15:38.363674 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_binary_with_plan_ref.py
+-rw-r--r--   0        0        0     3867 2021-12-02 09:15:38.359674 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_documents_with_many.py
+-rw-r--r--   0        0        0     4644 2021-12-02 09:15:38.367673 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_documents_with_plan_ref.py
+-rw-r--r--   0        0        0     3827 2021-12-02 09:15:38.347674 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_text_with_many.py
+-rw-r--r--   0        0        0     3965 2021-12-02 09:15:38.403674 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_text_with_plan_ref.py
+-rw-r--r--   0        0        0     4246 2021-12-02 09:15:38.383674 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_text.py
+-rw-r--r--   0        0        0     4524 2021-12-02 09:15:38.583673 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_text_with.py
+-rw-r--r--   0        0        0     4398 2021-12-02 09:15:38.559673 sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_text_with_many.py
+-rw-r--r--   0        0        0     3901 2021-12-02 09:15:38.551673 sherpa-client-0.9.6/sherpa_client/api/annotate/format_binary.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.575701 sherpa-client-0.9.6/sherpa_client/api/annotations/__init__.py
+-rw-r--r--   0        0        0     2623 2021-12-02 09:15:38.547673 sherpa-client-0.9.6/sherpa_client/api/annotations/annotation_creators_count.py
+-rw-r--r--   0        0        0     3661 2021-12-02 09:15:38.579673 sherpa-client-0.9.6/sherpa_client/api/annotations/clear_annotations.py
+-rw-r--r--   0        0        0     3661 2021-12-02 09:15:38.571673 sherpa-client-0.9.6/sherpa_client/api/annotations/count_annotations.py
+-rw-r--r--   0        0        0     2590 2021-12-02 09:15:38.503673 sherpa-client-0.9.6/sherpa_client/api/annotations/create_annotation.py
+-rw-r--r--   0        0        0     2546 2021-12-02 09:15:38.563673 sherpa-client-0.9.6/sherpa_client/api/annotations/delete_annotation.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.611701 sherpa-client-0.9.6/sherpa_client/api/annotators/__init__.py
+-rw-r--r--   0        0        0     2267 2021-12-02 09:15:38.515673 sherpa-client-0.9.6/sherpa_client/api/annotators/get_annotators_by_type.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.531702 sherpa-client-0.9.6/sherpa_client/api/authentication/__init__.py
+-rw-r--r--   0        0        0     4771 2021-12-02 09:15:38.635673 sherpa-client-0.9.6/sherpa_client/api/authentication/request_jwt_token.py
+-rw-r--r--   0        0        0     1243 2021-12-02 09:15:38.467673 sherpa-client-0.9.6/sherpa_client/api/authentication/user_sign_out.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.603701 sherpa-client-0.9.6/sherpa_client/api/categories/__init__.py
+-rw-r--r--   0        0        0     2622 2021-12-02 09:15:38.547673 sherpa-client-0.9.6/sherpa_client/api/categories/category_creators_count.py
+-rw-r--r--   0        0        0     3660 2021-12-02 09:15:38.679672 sherpa-client-0.9.6/sherpa_client/api/categories/count_categories.py
+-rw-r--r--   0        0        0     2557 2021-12-02 09:15:38.639673 sherpa-client-0.9.6/sherpa_client/api/categories/create_document_category.py
+-rw-r--r--   0        0        0     3660 2021-12-02 09:15:38.739672 sherpa-client-0.9.6/sherpa_client/api/categories/delete_categories.py
+-rw-r--r--   0        0        0     2671 2021-12-02 09:15:38.707672 sherpa-client-0.9.6/sherpa_client/api/categories/delete_category.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.631701 sherpa-client-0.9.6/sherpa_client/api/documents/__init__.py
+-rw-r--r--   0        0        0     2512 2021-12-02 09:15:38.715672 sherpa-client-0.9.6/sherpa_client/api/documents/delete_document.py
+-rw-r--r--   0        0        0     3416 2021-12-02 09:15:38.771672 sherpa-client-0.9.6/sherpa_client/api/documents/export_documents.py
+-rw-r--r--   0        0        0     3069 2021-12-02 09:15:38.739672 sherpa-client-0.9.6/sherpa_client/api/documents/export_documents_sample.py
+-rw-r--r--   0        0        0     3604 2021-12-02 09:15:38.803672 sherpa-client-0.9.6/sherpa_client/api/documents/get_document.py
+-rw-r--r--   0        0        0     2529 2021-12-02 09:15:38.719672 sherpa-client-0.9.6/sherpa_client/api/documents/index_document.py
+-rw-r--r--   0        0        0     6566 2021-12-02 09:15:38.891672 sherpa-client-0.9.6/sherpa_client/api/documents/launch_document_import.py
+-rw-r--r--   0        0        0     6698 2021-12-02 09:15:38.931671 sherpa-client-0.9.6/sherpa_client/api/documents/launch_uploaded_document_import.py
+-rw-r--r--   0        0        0     4802 2021-12-02 09:15:38.931671 sherpa-client-0.9.6/sherpa_client/api/documents/search_and_delete_documents.py
+-rw-r--r--   0        0        0     5058 2021-12-02 09:15:38.943672 sherpa-client-0.9.6/sherpa_client/api/documents/search_and_export_documents.py
+-rw-r--r--   0        0        0     5201 2021-12-02 09:15:38.983671 sherpa-client-0.9.6/sherpa_client/api/documents/search_and_tag_documents.py
+-rw-r--r--   0        0        0     6569 2021-12-02 09:15:39.159671 sherpa-client-0.9.6/sherpa_client/api/documents/search_documents.py
+-rw-r--r--   0        0        0     2025 2021-12-02 09:15:38.843672 sherpa-client-0.9.6/sherpa_client/api/documents/set_metadata_on_document.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.647701 sherpa-client-0.9.6/sherpa_client/api/experiments/__init__.py
+-rw-r--r--   0        0        0     1554 2021-12-02 09:15:38.815672 sherpa-client-0.9.6/sherpa_client/api/experiments/cancel_experiment.py
+-rw-r--r--   0        0        0     2658 2021-12-02 09:15:38.891672 sherpa-client-0.9.6/sherpa_client/api/experiments/compute_experiment_label_hint.py
+-rw-r--r--   0        0        0     2594 2021-12-02 09:15:38.875672 sherpa-client-0.9.6/sherpa_client/api/experiments/create_experiment.py
+-rw-r--r--   0        0        0     2584 2021-12-02 09:15:38.923672 sherpa-client-0.9.6/sherpa_client/api/experiments/delete_experiment.py
+-rw-r--r--   0        0        0     2585 2021-12-02 09:15:38.979671 sherpa-client-0.9.6/sherpa_client/api/experiments/delete_experiments.py
+-rw-r--r--   0        0        0     2541 2021-12-02 09:15:39.039671 sherpa-client-0.9.6/sherpa_client/api/experiments/get_experiment.py
+-rw-r--r--   0        0        0     2513 2021-12-02 09:15:39.003671 sherpa-client-0.9.6/sherpa_client/api/experiments/get_experiments.py
+-rw-r--r--   0        0        0     2594 2021-12-02 09:15:39.039671 sherpa-client-0.9.6/sherpa_client/api/experiments/launch_experiment.py
+-rw-r--r--   0        0        0     2545 2021-12-02 09:15:39.035671 sherpa-client-0.9.6/sherpa_client/api/experiments/patch_experiment.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.659701 sherpa-client-0.9.6/sherpa_client/api/gazetteers/__init__.py
+-rw-r--r--   0        0        0     1565 2021-12-02 09:15:38.983671 sherpa-client-0.9.6/sherpa_client/api/gazetteers/cancel_synchronize_gazetteer.py
+-rw-r--r--   0        0        0     2657 2021-12-02 09:15:39.083671 sherpa-client-0.9.6/sherpa_client/api/gazetteers/compute_gazetteer_label_hint.py
+-rw-r--r--   0        0        0     2586 2021-12-02 09:15:39.071671 sherpa-client-0.9.6/sherpa_client/api/gazetteers/create_gazetteer.py
+-rw-r--r--   0        0        0     2583 2021-12-02 09:15:39.131671 sherpa-client-0.9.6/sherpa_client/api/gazetteers/delete_gazetteer.py
+-rw-r--r--   0        0        0     2584 2021-12-02 09:15:39.087671 sherpa-client-0.9.6/sherpa_client/api/gazetteers/delete_gazetteers.py
+-rw-r--r--   0        0        0     2343 2021-12-02 09:15:39.139671 sherpa-client-0.9.6/sherpa_client/api/gazetteers/export_gazetteer.py
+-rw-r--r--   0        0        0     2731 2021-12-02 09:15:39.215670 sherpa-client-0.9.6/sherpa_client/api/gazetteers/export_gazetteers.py
+-rw-r--r--   0        0        0     2531 2021-12-02 09:15:39.187671 sherpa-client-0.9.6/sherpa_client/api/gazetteers/get_gazetteer.py
+-rw-r--r--   0        0        0     2499 2021-12-02 09:15:39.159671 sherpa-client-0.9.6/sherpa_client/api/gazetteers/get_gazetteers.py
+-rw-r--r--   0        0        0     2535 2021-12-02 09:15:39.187671 sherpa-client-0.9.6/sherpa_client/api/gazetteers/patch_gazetteer.py
+-rw-r--r--   0        0        0     2598 2021-12-02 09:15:39.191671 sherpa-client-0.9.6/sherpa_client/api/gazetteers/synchronize_gazetteer.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.655701 sherpa-client-0.9.6/sherpa_client/api/groups/__init__.py
+-rw-r--r--   0        0        0     2266 2021-12-02 09:15:39.223671 sherpa-client-0.9.6/sherpa_client/api/groups/add_group.py
+-rw-r--r--   0        0        0     2921 2021-12-02 09:15:39.263670 sherpa-client-0.9.6/sherpa_client/api/groups/delete_group.py
+-rw-r--r--   0        0        0     2314 2021-12-02 09:15:39.243670 sherpa-client-0.9.6/sherpa_client/api/groups/get_group.py
+-rw-r--r--   0        0        0     2192 2021-12-02 09:15:39.207671 sherpa-client-0.9.6/sherpa_client/api/groups/get_groups.py
+-rw-r--r--   0        0        0     2263 2021-12-02 09:15:39.303670 sherpa-client-0.9.6/sherpa_client/api/groups/patch_group.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.639701 sherpa-client-0.9.6/sherpa_client/api/jobs/__init__.py
+-rw-r--r--   0        0        0     2293 2021-12-02 09:15:39.327670 sherpa-client-0.9.6/sherpa_client/api/jobs/cancel_global_job.py
+-rw-r--r--   0        0        0     2600 2021-12-02 09:15:39.319670 sherpa-client-0.9.6/sherpa_client/api/jobs/cancel_job.py
+-rw-r--r--   0        0        0     2896 2021-12-02 09:15:39.399670 sherpa-client-0.9.6/sherpa_client/api/jobs/get_all_jobs.py
+-rw-r--r--   0        0        0     2287 2021-12-02 09:15:39.371670 sherpa-client-0.9.6/sherpa_client/api/jobs/get_global_job.py
+-rw-r--r--   0        0        0     2594 2021-12-02 09:15:39.335670 sherpa-client-0.9.6/sherpa_client/api/jobs/get_job.py
+-rw-r--r--   0        0        0     3204 2021-12-02 09:15:39.383670 sherpa-client-0.9.6/sherpa_client/api/jobs/get_jobs.py
+-rw-r--r--   0        0        0     3306 2021-12-02 09:15:39.387670 sherpa-client-0.9.6/sherpa_client/api/jobs/launch_dummy_job.py
+-rw-r--r--   0        0        0     2616 2021-12-02 09:15:39.419670 sherpa-client-0.9.6/sherpa_client/api/jobs/wait_for_job.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.659701 sherpa-client-0.9.6/sherpa_client/api/labels/__init__.py
+-rw-r--r--   0        0        0     2536 2021-12-02 09:15:39.383670 sherpa-client-0.9.6/sherpa_client/api/labels/create_label.py
+-rw-r--r--   0        0        0     2687 2021-12-02 09:15:39.395670 sherpa-client-0.9.6/sherpa_client/api/labels/delete_label_by_name.py
+-rw-r--r--   0        0        0     3067 2021-12-02 09:15:39.451670 sherpa-client-0.9.6/sherpa_client/api/labels/get_labels.py
+-rw-r--r--   0        0        0     2808 2021-12-02 09:15:39.559669 sherpa-client-0.9.6/sherpa_client/api/labels/update_label.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.595701 sherpa-client-0.9.6/sherpa_client/api/lexicons/__init__.py
+-rw-r--r--   0        0        0     2726 2021-12-02 09:15:39.463670 sherpa-client-0.9.6/sherpa_client/api/lexicons/create_lexicon.py
+-rw-r--r--   0        0        0     2941 2021-12-02 09:15:39.555669 sherpa-client-0.9.6/sherpa_client/api/lexicons/create_term.py
+-rw-r--r--   0        0        0     2621 2021-12-02 09:15:39.491670 sherpa-client-0.9.6/sherpa_client/api/lexicons/delete_lexicon_by_name.py
+-rw-r--r--   0        0        0     3298 2021-12-02 09:15:39.563669 sherpa-client-0.9.6/sherpa_client/api/lexicons/get_lexicon.py
+-rw-r--r--   0        0        0     3125 2021-12-02 09:15:39.551669 sherpa-client-0.9.6/sherpa_client/api/lexicons/get_lexicons.py
+-rw-r--r--   0        0        0     3089 2021-12-02 09:15:39.563669 sherpa-client-0.9.6/sherpa_client/api/lexicons/launch_uploaded_terms_import.py
+-rw-r--r--   0        0        0     6091 2021-12-02 09:15:39.851668 sherpa-client-0.9.6/sherpa_client/api/lexicons/search_terms.py
+-rw-r--r--   0        0        0     2483 2021-12-02 09:15:39.547669 sherpa-client-0.9.6/sherpa_client/api/lexicons/update_lexicon.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.555702 sherpa-client-0.9.6/sherpa_client/api/metrics/__init__.py
+-rw-r--r--   0        0        0     2751 2021-12-02 09:15:39.595669 sherpa-client-0.9.6/sherpa_client/api/metrics/get_annotation_metrics.py
+-rw-r--r--   0        0        0     2733 2021-12-02 09:15:39.659669 sherpa-client-0.9.6/sherpa_client/api/metrics/get_categories_metrics.py
+-rw-r--r--   0        0        0     2711 2021-12-02 09:15:39.619669 sherpa-client-0.9.6/sherpa_client/api/metrics/get_corpus_metrics.py
+-rw-r--r--   0        0        0     2225 2021-12-02 09:15:39.591669 sherpa-client-0.9.6/sherpa_client/api/metrics/get_model_metrics.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.655701 sherpa-client-0.9.6/sherpa_client/api/models/__init__.py
+-rw-r--r--   0        0        0     1430 2021-12-02 09:15:39.575669 sherpa-client-0.9.6/sherpa_client/api/models/delete_models.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.559702 sherpa-client-0.9.6/sherpa_client/api/plans/__init__.py
+-rw-r--r--   0        0        0     2652 2021-12-02 09:15:39.695669 sherpa-client-0.9.6/sherpa_client/api/plans/compute_plan_label_hint.py
+-rw-r--r--   0        0        0     2653 2021-12-02 09:15:39.687669 sherpa-client-0.9.6/sherpa_client/api/plans/create_plan.py
+-rw-r--r--   0        0        0     2578 2021-12-02 09:15:39.759668 sherpa-client-0.9.6/sherpa_client/api/plans/delete_plan.py
+-rw-r--r--   0        0        0     2579 2021-12-02 09:15:39.843668 sherpa-client-0.9.6/sherpa_client/api/plans/delete_plans.py
+-rw-r--r--   0        0        0     2618 2021-12-02 09:15:39.715669 sherpa-client-0.9.6/sherpa_client/api/plans/get_plan.py
+-rw-r--r--   0        0        0     2664 2021-12-02 09:15:39.695669 sherpa-client-0.9.6/sherpa_client/api/plans/get_plans.py
+-rw-r--r--   0        0        0     2622 2021-12-02 09:15:39.723669 sherpa-client-0.9.6/sherpa_client/api/plans/patch_plan.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.611701 sherpa-client-0.9.6/sherpa_client/api/project_engines/__init__.py
+-rw-r--r--   0        0        0     3453 2021-12-02 09:15:39.771669 sherpa-client-0.9.6/sherpa_client/api/project_engines/get_project_engine_parameters_schema.py
+-rw-r--r--   0        0        0     2480 2021-12-02 09:15:39.751669 sherpa-client-0.9.6/sherpa_client/api/project_engines/get_project_engines.py
+-rw-r--r--   0        0        0     4454 2021-12-02 09:15:39.887668 sherpa-client-0.9.6/sherpa_client/api/project_engines/get_project_services.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.615701 sherpa-client-0.9.6/sherpa_client/api/projects/__init__.py
+-rw-r--r--   0        0        0     1694 2021-12-02 09:15:39.775668 sherpa-client-0.9.6/sherpa_client/api/projects/auto_discover_on_corpus.py
+-rw-r--r--   0        0        0     2089 2021-12-02 09:15:39.815668 sherpa-client-0.9.6/sherpa_client/api/projects/compute_train_test_split.py
+-rw-r--r--   0        0        0     2941 2021-12-02 09:15:39.887668 sherpa-client-0.9.6/sherpa_client/api/projects/create_project.py
+-rw-r--r--   0        0        0     4578 2021-12-02 09:15:39.959668 sherpa-client-0.9.6/sherpa_client/api/projects/create_project_from_archive.py
+-rw-r--r--   0        0        0     4301 2021-12-02 09:15:39.995668 sherpa-client-0.9.6/sherpa_client/api/projects/create_project_from_uploaded_archive.py
+-rw-r--r--   0        0        0     1927 2021-12-02 09:15:39.831668 sherpa-client-0.9.6/sherpa_client/api/projects/create_tour_project.py
+-rw-r--r--   0        0        0     2299 2021-12-02 09:15:39.891668 sherpa-client-0.9.6/sherpa_client/api/projects/delete_project.py
+-rw-r--r--   0        0        0     2098 2021-12-02 09:15:39.899668 sherpa-client-0.9.6/sherpa_client/api/projects/delete_tour_project.py
+-rw-r--r--   0        0        0     2545 2021-12-02 09:15:39.927668 sherpa-client-0.9.6/sherpa_client/api/projects/deploy_project.py
+-rw-r--r--   0        0        0     2470 2021-12-02 09:15:39.919668 sherpa-client-0.9.6/sherpa_client/api/projects/export_dataset.py
+-rw-r--r--   0        0        0     3124 2021-12-02 09:15:40.059667 sherpa-client-0.9.6/sherpa_client/api/projects/export_models.py
+-rw-r--r--   0        0        0     2779 2021-12-02 09:15:39.999668 sherpa-client-0.9.6/sherpa_client/api/projects/export_project.py
+-rw-r--r--   0        0        0     2079 2021-12-02 09:15:40.015668 sherpa-client-0.9.6/sherpa_client/api/projects/flush_indices.py
+-rw-r--r--   0        0        0     1998 2021-12-02 09:15:39.955668 sherpa-client-0.9.6/sherpa_client/api/projects/get_app_state.py
+-rw-r--r--   0        0        0     2201 2021-12-02 09:15:40.043667 sherpa-client-0.9.6/sherpa_client/api/projects/get_config.py
+-rw-r--r--   0        0        0     2649 2021-12-02 09:15:40.027668 sherpa-client-0.9.6/sherpa_client/api/projects/get_metadata_definition.py
+-rw-r--r--   0        0        0     3786 2021-12-02 09:15:40.115667 sherpa-client-0.9.6/sherpa_client/api/projects/get_project_info.py
+-rw-r--r--   0        0        0     4644 2021-12-02 09:15:40.227667 sherpa-client-0.9.6/sherpa_client/api/projects/get_projects.py
+-rw-r--r--   0        0        0     2241 2021-12-02 09:15:40.055667 sherpa-client-0.9.6/sherpa_client/api/projects/get_properties.py
+-rw-r--r--   0        0        0     2927 2021-12-02 09:15:40.095667 sherpa-client-0.9.6/sherpa_client/api/projects/import_archive.py
+-rw-r--r--   0        0        0     2916 2021-12-02 09:15:40.095667 sherpa-client-0.9.6/sherpa_client/api/projects/import_models.py
+-rw-r--r--   0        0        0     3004 2021-12-02 09:15:40.107667 sherpa-client-0.9.6/sherpa_client/api/projects/import_uploaded_archive.py
+-rw-r--r--   0        0        0     3000 2021-12-02 09:15:40.163667 sherpa-client-0.9.6/sherpa_client/api/projects/import_uploaded_models.py
+-rw-r--r--   0        0        0     2714 2021-12-02 09:15:40.163667 sherpa-client-0.9.6/sherpa_client/api/projects/launch_project_reindexing.py
+-rw-r--r--   0        0        0     2967 2021-12-02 09:15:40.179667 sherpa-client-0.9.6/sherpa_client/api/projects/launch_project_restoration_from_backup.py
+-rw-r--r--   0        0        0     2677 2021-12-02 09:15:40.171667 sherpa-client-0.9.6/sherpa_client/api/projects/launch_project_restoration_from_image.py
+-rw-r--r--   0        0        0     5107 2021-12-02 09:15:40.319666 sherpa-client-0.9.6/sherpa_client/api/projects/maybe_create_projects_and_import_models_from_archive.py
+-rw-r--r--   0        0        0     2415 2021-12-02 09:15:40.227667 sherpa-client-0.9.6/sherpa_client/api/projects/reindex_projects.py
+-rw-r--r--   0        0        0     2456 2021-12-02 09:15:40.303667 sherpa-client-0.9.6/sherpa_client/api/projects/undeploy_project.py
+-rw-r--r--   0        0        0     1428 2021-12-02 09:15:40.231667 sherpa-client-0.9.6/sherpa_client/api/projects/update_config_options.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.651701 sherpa-client-0.9.6/sherpa_client/api/roles/__init__.py
+-rw-r--r--   0        0        0     3191 2021-12-02 09:15:40.291667 sherpa-client-0.9.6/sherpa_client/api/roles/add_role.py
+-rw-r--r--   0        0        0     2234 2021-12-02 09:15:40.243667 sherpa-client-0.9.6/sherpa_client/api/roles/delete_role.py
+-rw-r--r--   0        0        0     1845 2021-12-02 09:15:40.231667 sherpa-client-0.9.6/sherpa_client/api/roles/get_permissions.py
+-rw-r--r--   0        0        0     2274 2021-12-02 09:15:40.295667 sherpa-client-0.9.6/sherpa_client/api/roles/get_role.py
+-rw-r--r--   0        0        0     2178 2021-12-02 09:15:40.283667 sherpa-client-0.9.6/sherpa_client/api/roles/get_roles.py
+-rw-r--r--   0        0        0     2232 2021-12-02 09:15:40.307667 sherpa-client-0.9.6/sherpa_client/api/roles/update_role.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.607701 sherpa-client-0.9.6/sherpa_client/api/segments/__init__.py
+-rw-r--r--   0        0        0     7194 2021-12-02 09:15:40.699665 sherpa-client-0.9.6/sherpa_client/api/segments/find_similar_segments.py
+-rw-r--r--   0        0        0     6738 2021-12-02 09:15:40.595666 sherpa-client-0.9.6/sherpa_client/api/segments/get_segment_context.py
+-rw-r--r--   0        0        0     6559 2021-12-02 09:15:40.623665 sherpa-client-0.9.6/sherpa_client/api/segments/search_segments.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.571701 sherpa-client-0.9.6/sherpa_client/api/services/__init__.py
+-rw-r--r--   0        0        0     3529 2021-12-02 09:15:40.431666 sherpa-client-0.9.6/sherpa_client/api/services/get_engine_parameters_schema.py
+-rw-r--r--   0        0        0     7071 2021-12-02 09:15:40.883664 sherpa-client-0.9.6/sherpa_client/api/services/get_services.py
+-rw-r--r--   0        0        0     6778 2021-12-02 09:15:40.851665 sherpa-client-0.9.6/sherpa_client/api/services/get_services_distinct_values.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.591701 sherpa-client-0.9.6/sherpa_client/api/shares/__init__.py
+-rw-r--r--   0        0        0     1879 2021-12-02 09:15:40.399666 sherpa-client-0.9.6/sherpa_client/api/shares/change_project_ownership.py
+-rw-r--r--   0        0        0     1610 2021-12-02 09:15:40.379666 sherpa-client-0.9.6/sherpa_client/api/shares/delete_share_with_group.py
+-rw-r--r--   0        0        0     1591 2021-12-02 09:15:40.399666 sherpa-client-0.9.6/sherpa_client/api/shares/delete_share_with_user.py
+-rw-r--r--   0        0        0     2550 2021-12-02 09:15:40.487666 sherpa-client-0.9.6/sherpa_client/api/shares/get_group_shares.py
+-rw-r--r--   0        0        0     2549 2021-12-02 09:15:40.439666 sherpa-client-0.9.6/sherpa_client/api/shares/get_user_shares.py
+-rw-r--r--   0        0        0     2096 2021-12-02 09:15:40.427666 sherpa-client-0.9.6/sherpa_client/api/shares/share_with_group.py
+-rw-r--r--   0        0        0     1980 2021-12-02 09:15:40.491666 sherpa-client-0.9.6/sherpa_client/api/shares/share_with_user.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.563701 sherpa-client-0.9.6/sherpa_client/api/suggesters/__init__.py
+-rw-r--r--   0        0        0     2657 2021-12-02 09:15:40.535666 sherpa-client-0.9.6/sherpa_client/api/suggesters/compute_suggester_label_hint.py
+-rw-r--r--   0        0        0     2586 2021-12-02 09:15:40.715665 sherpa-client-0.9.6/sherpa_client/api/suggesters/create_suggester.py
+-rw-r--r--   0        0        0     2583 2021-12-02 09:15:40.559666 sherpa-client-0.9.6/sherpa_client/api/suggesters/delete_suggester.py
+-rw-r--r--   0        0        0     2584 2021-12-02 09:15:40.583666 sherpa-client-0.9.6/sherpa_client/api/suggesters/delete_suggesters.py
+-rw-r--r--   0        0        0     2531 2021-12-02 09:15:40.599665 sherpa-client-0.9.6/sherpa_client/api/suggesters/get_suggester.py
+-rw-r--r--   0        0        0     2499 2021-12-02 09:15:40.623665 sherpa-client-0.9.6/sherpa_client/api/suggesters/get_suggesters.py
+-rw-r--r--   0        0        0     2535 2021-12-02 09:15:40.659665 sherpa-client-0.9.6/sherpa_client/api/suggesters/patch_suggester.py
+-rw-r--r--   0        0        0     2500 2021-12-02 09:15:40.767665 sherpa-client-0.9.6/sherpa_client/api/suggesters/start_suggester.py
+-rw-r--r--   0        0        0     1551 2021-12-02 09:15:40.659665 sherpa-client-0.9.6/sherpa_client/api/suggesters/stop_suggester.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.567701 sherpa-client-0.9.6/sherpa_client/api/suggestions/__init__.py
+-rw-r--r--   0        0        0     2242 2021-12-02 09:15:40.719665 sherpa-client-0.9.6/sherpa_client/api/suggestions/clear_suggestions.py
+-rw-r--r--   0        0        0     2640 2021-12-02 09:15:40.743665 sherpa-client-0.9.6/sherpa_client/api/suggestions/delete_suggestion.py
+-rw-r--r--   0        0        0     4581 2021-12-02 09:15:40.875665 sherpa-client-0.9.6/sherpa_client/api/suggestions/get_suggestions.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.555702 sherpa-client-0.9.6/sherpa_client/api/uploads/__init__.py
+-rw-r--r--   0        0        0     2253 2021-12-02 09:15:40.763665 sherpa-client-0.9.6/sherpa_client/api/uploads/get_uploaded_file_info.py
+-rw-r--r--   0        0        0     3621 2021-12-02 09:15:40.815665 sherpa-client-0.9.6/sherpa_client/api/uploads/upload_files.py
+-rw-r--r--   0        0        0        0 2021-12-02 09:15:30.599701 sherpa-client-0.9.6/sherpa_client/api/users/__init__.py
+-rw-r--r--   0        0        0     2830 2021-12-02 09:15:40.835665 sherpa-client-0.9.6/sherpa_client/api/users/add_user.py
+-rw-r--r--   0        0        0     2234 2021-12-02 09:15:40.775665 sherpa-client-0.9.6/sherpa_client/api/users/delete_user.py
+-rw-r--r--   0        0        0     3288 2021-12-02 09:15:40.899664 sherpa-client-0.9.6/sherpa_client/api/users/get_user.py
+-rw-r--r--   0        0        0     3245 2021-12-02 09:15:40.939664 sherpa-client-0.9.6/sherpa_client/api/users/get_users.py
+-rw-r--r--   0        0        0     2232 2021-12-02 09:15:40.883664 sherpa-client-0.9.6/sherpa_client/api/users/update_permissions.py
+-rw-r--r--   0        0        0     2240 2021-12-02 09:15:40.927664 sherpa-client-0.9.6/sherpa_client/api/users/update_profile.py
+-rw-r--r--   0        0        0     2697 2021-12-02 12:15:29.597648 sherpa-client-0.9.6/sherpa_client/client.py
+-rw-r--r--   0        0        0     8820 2021-12-02 09:15:37.867675 sherpa-client-0.9.6/sherpa_client/models/__init__.py
+-rw-r--r--   0        0        0      580 2021-12-02 09:15:40.819665 sherpa-client-0.9.6/sherpa_client/models/ack.py
+-rw-r--r--   0        0        0     1133 2021-12-02 09:15:40.911664 sherpa-client-0.9.6/sherpa_client/models/aggregation.py
+-rw-r--r--   0        0        0     2232 2021-12-02 09:15:40.959664 sherpa-client-0.9.6/sherpa_client/models/annotate_binary_form.py
+-rw-r--r--   0        0        0     2315 2021-12-02 09:15:40.967664 sherpa-client-0.9.6/sherpa_client/models/annotate_binary_with_plan_ref_multipart_data.py
+-rw-r--r--   0        0        0     2505 2021-12-02 09:15:40.991664 sherpa-client-0.9.6/sherpa_client/models/annotate_documents_with_many.py
+-rw-r--r--   0        0        0     2348 2021-12-02 09:15:40.995664 sherpa-client-0.9.6/sherpa_client/models/annotate_format_binary_with_plan_ref_multipart_data.py
+-rw-r--r--   0        0        0     2038 2021-12-02 09:15:40.971664 sherpa-client-0.9.6/sherpa_client/models/annotate_text_with_many.py
+-rw-r--r--   0        0        0     3199 2021-12-02 09:15:41.083664 sherpa-client-0.9.6/sherpa_client/models/annotated_doc_annotation.py
+-rw-r--r--   0        0        0     1279 2021-12-02 09:15:40.951664 sherpa-client-0.9.6/sherpa_client/models/annotated_doc_annotation_properties.py
+-rw-r--r--   0        0        0     2124 2021-12-02 09:15:40.999664 sherpa-client-0.9.6/sherpa_client/models/annotated_doc_category.py
+-rw-r--r--   0        0        0     1269 2021-12-02 09:15:40.971664 sherpa-client-0.9.6/sherpa_client/models/annotated_doc_category_properties.py
+-rw-r--r--   0        0        0     4262 2021-12-02 09:15:41.131664 sherpa-client-0.9.6/sherpa_client/models/annotated_document.py
+-rw-r--r--   0        0        0     1237 2021-12-02 09:15:41.007664 sherpa-client-0.9.6/sherpa_client/models/annotated_document_metadata.py
+-rw-r--r--   0        0        0     1911 2021-12-02 09:15:41.147664 sherpa-client-0.9.6/sherpa_client/models/annotation.py
+-rw-r--r--   0        0        0     1498 2021-12-02 09:15:41.031664 sherpa-client-0.9.6/sherpa_client/models/annotation_facets.py
+-rw-r--r--   0        0        0      716 2021-12-02 09:15:40.999664 sherpa-client-0.9.6/sherpa_client/models/annotation_id.py
+-rw-r--r--   0        0        0     2513 2021-12-02 09:15:41.063664 sherpa-client-0.9.6/sherpa_client/models/annotation_metrics.py
+-rw-r--r--   0        0        0     3107 2021-12-02 09:15:41.131664 sherpa-client-0.9.6/sherpa_client/models/annotation_plan.py
+-rw-r--r--   0        0        0      149 2021-12-02 09:15:40.991664 sherpa-client-0.9.6/sherpa_client/models/annotation_status.py
+-rw-r--r--   0        0        0     2064 2021-12-02 09:15:41.103664 sherpa-client-0.9.6/sherpa_client/models/annotation_term.py
+-rw-r--r--   0        0        0     1237 2021-12-02 09:15:41.127664 sherpa-client-0.9.6/sherpa_client/models/annotation_term_properties.py
+-rw-r--r--   0        0        0     1411 2021-12-02 13:41:50.489601 sherpa-client-0.9.6/sherpa_client/models/annotator.py
+-rw-r--r--   0        0        0     2007 2021-12-02 09:15:41.095664 sherpa-client-0.9.6/sherpa_client/models/annotator_multimap.py
+-rw-r--r--   0        0        0     1044 2021-12-02 12:30:35.358108 sherpa-client-0.9.6/sherpa_client/models/bearer_token.py
+-rw-r--r--   0        0        0      767 2021-12-02 09:15:41.059664 sherpa-client-0.9.6/sherpa_client/models/bucket.py
+-rw-r--r--   0        0        0     1029 2021-12-02 09:15:41.087664 sherpa-client-0.9.6/sherpa_client/models/categories_facets.py
+-rw-r--r--   0        0        0     1726 2021-12-02 09:15:41.147664 sherpa-client-0.9.6/sherpa_client/models/category.py
+-rw-r--r--   0        0        0      681 2021-12-02 09:15:41.111664 sherpa-client-0.9.6/sherpa_client/models/category_id.py
+-rw-r--r--   0        0        0     1679 2021-12-02 09:15:41.135664 sherpa-client-0.9.6/sherpa_client/models/category_metrics.py
+-rw-r--r--   0        0        0      147 2021-12-02 09:15:41.087664 sherpa-client-0.9.6/sherpa_client/models/category_status.py
+-rw-r--r--   0        0        0      785 2021-12-02 09:15:41.127664 sherpa-client-0.9.6/sherpa_client/models/classification_config.py
+-rw-r--r--   0        0        0      874 2021-12-02 09:15:41.147664 sherpa-client-0.9.6/sherpa_client/models/classification_options.py
+-rw-r--r--   0        0        0     2074 2021-12-02 09:15:41.211663 sherpa-client-0.9.6/sherpa_client/models/config_patch_options.py
+-rw-r--r--   0        0        0     2164 2021-12-02 09:15:41.239663 sherpa-client-0.9.6/sherpa_client/models/convert_annotation_plan.py
+-rw-r--r--   0        0        0     2436 2021-12-02 09:15:41.215663 sherpa-client-0.9.6/sherpa_client/models/convert_format_annotation_plan.py
+-rw-r--r--   0        0        0     1322 2021-12-02 09:15:41.195663 sherpa-client-0.9.6/sherpa_client/models/converter.py
+-rw-r--r--   0        0        0     1217 2021-12-02 09:15:41.223663 sherpa-client-0.9.6/sherpa_client/models/converter_parameters.py
+-rw-r--r--   0        0        0     1430 2021-12-02 09:15:41.219663 sherpa-client-0.9.6/sherpa_client/models/corpus_metrics.py
+-rw-r--r--   0        0        0     1219 2021-12-02 09:15:41.199663 sherpa-client-0.9.6/sherpa_client/models/create_lexicon_response_200.py
+-rw-r--r--   0        0        0     2307 2021-12-02 09:15:41.283663 sherpa-client-0.9.6/sherpa_client/models/create_project_from_archive_multipart_data.py
+-rw-r--r--   0        0        0     1204 2021-12-02 09:15:41.203663 sherpa-client-0.9.6/sherpa_client/models/create_term_response_200.py
+-rw-r--r--   0        0        0      828 2021-12-02 09:15:41.195663 sherpa-client-0.9.6/sherpa_client/models/created_by_count.py
+-rw-r--r--   0        0        0      796 2021-12-02 09:15:41.199663 sherpa-client-0.9.6/sherpa_client/models/credentials.py
+-rw-r--r--   0        0        0      964 2021-12-02 09:15:41.207663 sherpa-client-0.9.6/sherpa_client/models/delete_group_result.py
+-rw-r--r--   0        0        0     1392 2021-12-02 09:15:41.271663 sherpa-client-0.9.6/sherpa_client/models/delete_response.py
+-rw-r--r--   0        0        0     2727 2021-12-02 09:15:41.379663 sherpa-client-0.9.6/sherpa_client/models/doc_annotation.py
+-rw-r--r--   0        0        0      152 2021-12-02 09:15:41.207663 sherpa-client-0.9.6/sherpa_client/models/doc_annotation_status.py
+-rw-r--r--   0        0        0     2469 2021-12-02 09:15:41.359663 sherpa-client-0.9.6/sherpa_client/models/doc_category.py
+-rw-r--r--   0        0        0      150 2021-12-02 09:15:41.215663 sherpa-client-0.9.6/sherpa_client/models/doc_category_status.py
+-rw-r--r--   0        0        0      753 2021-12-02 09:15:41.259663 sherpa-client-0.9.6/sherpa_client/models/doc_sentence.py
+-rw-r--r--   0        0        0     4755 2021-12-02 09:15:41.455663 sherpa-client-0.9.6/sherpa_client/models/document.py
+-rw-r--r--   0        0        0     1191 2021-12-02 09:15:41.279663 sherpa-client-0.9.6/sherpa_client/models/document_facets.py
+-rw-r--r--   0        0        0      981 2021-12-02 09:15:41.275663 sherpa-client-0.9.6/sherpa_client/models/document_hit.py
+-rw-r--r--   0        0        0     2313 2021-12-02 09:15:41.423663 sherpa-client-0.9.6/sherpa_client/models/document_hits.py
+-rw-r--r--   0        0        0     1189 2021-12-02 09:15:41.331663 sherpa-client-0.9.6/sherpa_client/models/document_metadata.py
+-rw-r--r--   0        0        0      757 2021-12-02 09:15:41.299663 sherpa-client-0.9.6/sherpa_client/models/engine_config.py
+-rw-r--r--   0        0        0     2126 2021-12-02 09:15:41.367663 sherpa-client-0.9.6/sherpa_client/models/engine_config_import_summary.py
+-rw-r--r--   0        0        0      627 2021-12-02 09:15:41.311663 sherpa-client-0.9.6/sherpa_client/models/engine_name.py
+-rw-r--r--   0        0        0     2916 2021-12-02 09:15:41.443663 sherpa-client-0.9.6/sherpa_client/models/experiment.py
+-rw-r--r--   0        0        0     1193 2021-12-02 09:15:41.347663 sherpa-client-0.9.6/sherpa_client/models/experiment_parameters.py
+-rw-r--r--   0        0        0     1651 2021-12-02 09:15:41.371663 sherpa-client-0.9.6/sherpa_client/models/experiment_patch.py
+-rw-r--r--   0        0        0     1221 2021-12-02 09:15:41.367663 sherpa-client-0.9.6/sherpa_client/models/experiment_patch_parameters.py
+-rw-r--r--   0        0        0     2255 2021-12-02 09:15:41.487662 sherpa-client-0.9.6/sherpa_client/models/format_binary_form.py
+-rw-r--r--   0        0        0     2743 2021-12-02 09:15:41.455663 sherpa-client-0.9.6/sherpa_client/models/format_documents_with_many.py
+-rw-r--r--   0        0        0     2276 2021-12-02 09:15:41.475662 sherpa-client-0.9.6/sherpa_client/models/format_text_with_many.py
+-rw-r--r--   0        0        0     1322 2021-12-02 09:15:41.423663 sherpa-client-0.9.6/sherpa_client/models/formatter.py
+-rw-r--r--   0        0        0     1217 2021-12-02 09:15:41.443663 sherpa-client-0.9.6/sherpa_client/models/formatter_parameters.py
+-rw-r--r--   0        0        0     1962 2021-12-02 09:15:41.511662 sherpa-client-0.9.6/sherpa_client/models/gazetteer.py
+-rw-r--r--   0        0        0     1188 2021-12-02 09:15:41.439663 sherpa-client-0.9.6/sherpa_client/models/gazetteer_parameters.py
+-rw-r--r--   0        0        0     1412 2021-12-02 09:15:41.451662 sherpa-client-0.9.6/sherpa_client/models/gazetteer_patch.py
+-rw-r--r--   0        0        0     1216 2021-12-02 09:15:41.463662 sherpa-client-0.9.6/sherpa_client/models/gazetteer_patch_parameters.py
+-rw-r--r--   0        0        0      713 2021-12-02 09:15:41.463662 sherpa-client-0.9.6/sherpa_client/models/generated_label_hint.py
+-rw-r--r--   0        0        0     1212 2021-12-02 09:15:41.491662 sherpa-client-0.9.6/sherpa_client/models/get_app_state_response_200.py
+-rw-r--r--   0        0        0     1285 2021-12-02 09:15:41.511662 sherpa-client-0.9.6/sherpa_client/models/get_engine_parameters_schema_response_200.py
+-rw-r--r--   0        0        0     1323 2021-12-02 09:15:41.511662 sherpa-client-0.9.6/sherpa_client/models/get_project_engine_parameters_schema_response_200.py
+-rw-r--r--   0        0        0      217 2021-12-02 09:15:41.463662 sherpa-client-0.9.6/sherpa_client/models/get_segment_context_context_output.py
+-rw-r--r--   0        0        0     1224 2021-12-02 09:15:41.519662 sherpa-client-0.9.6/sherpa_client/models/get_suggestions_response_200.py
+-rw-r--r--   0        0        0     2405 2021-12-02 09:15:41.599662 sherpa-client-0.9.6/sherpa_client/models/group_desc.py
+-rw-r--r--   0        0        0      623 2021-12-02 09:15:41.511662 sherpa-client-0.9.6/sherpa_client/models/group_name.py
+-rw-r--r--   0        0        0     1384 2021-12-02 09:15:41.639662 sherpa-client-0.9.6/sherpa_client/models/group_patch.py
+-rw-r--r--   0        0        0     1057 2021-12-02 09:15:41.527662 sherpa-client-0.9.6/sherpa_client/models/group_share.py
+-rw-r--r--   0        0        0     4418 2021-12-02 09:15:41.751661 sherpa-client-0.9.6/sherpa_client/models/http_service_metadata.py
+-rw-r--r--   0        0        0     1244 2021-12-02 09:15:41.535662 sherpa-client-0.9.6/sherpa_client/models/http_service_metadata_operations.py
+-rw-r--r--   0        0        0     1401 2021-12-02 09:15:41.583662 sherpa-client-0.9.6/sherpa_client/models/http_service_record.py
+-rw-r--r--   0        0        0     2246 2021-12-02 09:15:41.647662 sherpa-client-0.9.6/sherpa_client/models/import_archive_multipart_data.py
+-rw-r--r--   0        0        0     2241 2021-12-02 09:15:41.643662 sherpa-client-0.9.6/sherpa_client/models/import_models_multipart_data.py
+-rw-r--r--   0        0        0     4152 2021-12-02 09:15:41.767661 sherpa-client-0.9.6/sherpa_client/models/input_document.py
+-rw-r--r--   0        0        0     1217 2021-12-02 09:15:41.579662 sherpa-client-0.9.6/sherpa_client/models/input_document_metadata.py
+-rw-r--r--   0        0        0      636 2021-12-02 09:15:41.559662 sherpa-client-0.9.6/sherpa_client/models/input_label.py
+-rw-r--r--   0        0        0      452 2021-12-02 09:15:41.547662 sherpa-client-0.9.6/sherpa_client/models/job_status.py
+-rw-r--r--   0        0        0      444 2021-12-02 09:15:41.563662 sherpa-client-0.9.6/sherpa_client/models/job_type.py
+-rw-r--r--   0        0        0     1356 2021-12-02 09:15:41.619662 sherpa-client-0.9.6/sherpa_client/models/label.py
+-rw-r--r--   0        0        0      742 2021-12-02 09:15:41.599662 sherpa-client-0.9.6/sherpa_client/models/label_count.py
+-rw-r--r--   0        0        0     1162 2021-12-02 09:15:41.631662 sherpa-client-0.9.6/sherpa_client/models/label_update.py
+-rw-r--r--   0        0        0     2284 2021-12-02 09:15:41.699662 sherpa-client-0.9.6/sherpa_client/models/launch_document_import_multipart_data.py
+-rw-r--r--   0        0        0      323 2021-12-02 09:15:41.595662 sherpa-client-0.9.6/sherpa_client/models/launch_document_import_segmentation_policy.py
+-rw-r--r--   0        0        0     2360 2021-12-02 09:15:41.711662 sherpa-client-0.9.6/sherpa_client/models/launch_project_restoration_from_backup_multipart_data.py
+-rw-r--r--   0        0        0      331 2021-12-02 09:15:41.607662 sherpa-client-0.9.6/sherpa_client/models/launch_uploaded_document_import_segmentation_policy.py
+-rw-r--r--   0        0        0     2404 2021-12-02 09:15:41.731661 sherpa-client-0.9.6/sherpa_client/models/lexicon.py
+-rw-r--r--   0        0        0      921 2021-12-02 09:15:41.659662 sherpa-client-0.9.6/sherpa_client/models/lexicon_update.py
+-rw-r--r--   0        0        0     2424 2021-12-02 09:15:41.743661 sherpa-client-0.9.6/sherpa_client/models/maybe_create_projects_and_import_models_from_archive_multipart_data.py
+-rw-r--r--   0        0        0     1034 2021-12-02 09:15:41.719662 sherpa-client-0.9.6/sherpa_client/models/metadata_count.py
+-rw-r--r--   0        0        0     1132 2021-12-02 09:15:41.691662 sherpa-client-0.9.6/sherpa_client/models/metadata_definition.py
+-rw-r--r--   0        0        0     1461 2021-12-02 09:15:41.703662 sherpa-client-0.9.6/sherpa_client/models/metadata_definition_entry.py
+-rw-r--r--   0        0        0     2452 2021-12-02 09:15:41.787661 sherpa-client-0.9.6/sherpa_client/models/model_metrics.py
+-rw-r--r--   0        0        0     1191 2021-12-02 09:15:41.715662 sherpa-client-0.9.6/sherpa_client/models/model_metrics_options.py
+-rw-r--r--   0        0        0     2038 2021-12-02 09:15:41.783661 sherpa-client-0.9.6/sherpa_client/models/models_metrics.py
+-rw-r--r--   0        0        0     2351 2021-12-02 09:15:41.823661 sherpa-client-0.9.6/sherpa_client/models/named_annotation_plan.py
+-rw-r--r--   0        0        0     1101 2021-12-02 09:15:41.767661 sherpa-client-0.9.6/sherpa_client/models/new_experiment.py
+-rw-r--r--   0        0        0     1211 2021-12-02 09:15:41.791661 sherpa-client-0.9.6/sherpa_client/models/new_experiment_parameters.py
+-rw-r--r--   0        0        0     1093 2021-12-02 09:15:41.771661 sherpa-client-0.9.6/sherpa_client/models/new_gazetteer.py
+-rw-r--r--   0        0        0     1206 2021-12-02 09:15:41.783661 sherpa-client-0.9.6/sherpa_client/models/new_gazetteer_parameters.py
+-rw-r--r--   0        0        0     1361 2021-12-02 09:15:41.815661 sherpa-client-0.9.6/sherpa_client/models/new_group_desc.py
+-rw-r--r--   0        0        0      964 2021-12-02 09:15:41.783661 sherpa-client-0.9.6/sherpa_client/models/new_named_annotation_plan.py
+-rw-r--r--   0        0        0      844 2021-12-02 09:15:41.795661 sherpa-client-0.9.6/sherpa_client/models/new_role.py
+-rw-r--r--   0        0        0     1093 2021-12-02 09:15:41.811661 sherpa-client-0.9.6/sherpa_client/models/new_suggester.py
+-rw-r--r--   0        0        0     1206 2021-12-02 09:15:41.883661 sherpa-client-0.9.6/sherpa_client/models/new_suggester_parameters.py
+-rw-r--r--   0        0        0     1184 2021-12-02 09:15:41.839661 sherpa-client-0.9.6/sherpa_client/models/new_user.py
+-rw-r--r--   0        0        0      968 2021-12-02 09:15:41.831661 sherpa-client-0.9.6/sherpa_client/models/operation_count.py
+-rw-r--r--   0        0        0     1355 2021-12-02 09:15:41.867661 sherpa-client-0.9.6/sherpa_client/models/partial_label.py
+-rw-r--r--   0        0        0     1081 2021-12-02 09:15:41.851661 sherpa-client-0.9.6/sherpa_client/models/partial_lexicon.py
+-rw-r--r--   0        0        0     1571 2021-12-02 09:15:41.879661 sherpa-client-0.9.6/sherpa_client/models/plan_patch.py
+-rw-r--r--   0        0        0     6435 2021-12-02 09:15:42.163660 sherpa-client-0.9.6/sherpa_client/models/project_bean.py
+-rw-r--r--   0        0        0     3338 2021-12-02 09:15:42.011660 sherpa-client-0.9.6/sherpa_client/models/project_config_creation.py
+-rw-r--r--   0        0        0     1254 2021-12-02 09:15:41.863661 sherpa-client-0.9.6/sherpa_client/models/project_config_creation_properties.py
+-rw-r--r--   0        0        0      722 2021-12-02 09:15:41.855661 sherpa-client-0.9.6/sherpa_client/models/project_property.py
+-rw-r--r--   0        0        0     1536 2021-12-02 09:15:41.919661 sherpa-client-0.9.6/sherpa_client/models/project_status.py
+-rw-r--r--   0        0        0     1349 2021-12-02 09:15:41.911661 sherpa-client-0.9.6/sherpa_client/models/quality_figures.py
+-rw-r--r--   0        0        0      446 2021-12-02 09:15:41.859661 sherpa-client-0.9.6/sherpa_client/models/relation.py
+-rw-r--r--   0        0        0     3375 2021-12-02 09:15:42.055660 sherpa-client-0.9.6/sherpa_client/models/report.py
+-rw-r--r--   0        0        0     1550 2021-12-02 09:15:41.935661 sherpa-client-0.9.6/sherpa_client/models/report_classes.py
+-rw-r--r--   0        0        0      195 2021-12-02 09:15:41.871661 sherpa-client-0.9.6/sherpa_client/models/request_jwt_token_project_access_mode.py
+-rw-r--r--   0        0        0     2675 2021-12-02 09:15:42.043660 sherpa-client-0.9.6/sherpa_client/models/role_desc.py
+-rw-r--r--   0        0        0     1113 2021-12-02 09:15:41.943661 sherpa-client-0.9.6/sherpa_client/models/role_update.py
+-rw-r--r--   0        0        0      905 2021-12-02 09:15:41.919661 sherpa-client-0.9.6/sherpa_client/models/search_total.py
+-rw-r--r--   0        0        0      154 2021-12-02 09:15:41.879661 sherpa-client-0.9.6/sherpa_client/models/search_total_relation.py
+-rw-r--r--   0        0        0     3965 2021-12-02 09:15:42.087660 sherpa-client-0.9.6/sherpa_client/models/segment.py
+-rw-r--r--   0        0        0     1910 2021-12-02 09:15:42.039660 sherpa-client-0.9.6/sherpa_client/models/segment_context.py
+-rw-r--r--   0        0        0      944 2021-12-02 09:15:41.955661 sherpa-client-0.9.6/sherpa_client/models/segment_contexts.py
+-rw-r--r--   0        0        0      964 2021-12-02 09:15:41.971661 sherpa-client-0.9.6/sherpa_client/models/segment_hit.py
+-rw-r--r--   0        0        0     2305 2021-12-02 09:15:42.039660 sherpa-client-0.9.6/sherpa_client/models/segment_hits.py
+-rw-r--r--   0        0        0     1168 2021-12-02 09:15:42.003661 sherpa-client-0.9.6/sherpa_client/models/segment_metadata.py
+-rw-r--r--   0        0        0      756 2021-12-02 09:15:41.991660 sherpa-client-0.9.6/sherpa_client/models/share_mode.py
+-rw-r--r--   0        0        0     3251 2021-12-02 09:15:42.107660 sherpa-client-0.9.6/sherpa_client/models/sherpa_job_bean.py
+-rw-r--r--   0        0        0      248 2021-12-02 09:15:41.971661 sherpa-client-0.9.6/sherpa_client/models/sherpa_job_bean_status.py
+-rw-r--r--   0        0        0      642 2021-12-02 09:15:41.999661 sherpa-client-0.9.6/sherpa_client/models/sherpa_job_bean_type.py
+-rw-r--r--   0        0        0      883 2021-12-02 09:15:42.027660 sherpa-client-0.9.6/sherpa_client/models/simple_metadata.py
+-rw-r--r--   0        0        0     2111 2021-12-02 09:15:42.123660 sherpa-client-0.9.6/sherpa_client/models/suggester.py
+-rw-r--r--   0        0        0     1188 2021-12-02 09:15:42.063660 sherpa-client-0.9.6/sherpa_client/models/suggester_parameters.py
+-rw-r--r--   0        0        0     1412 2021-12-02 09:15:42.091660 sherpa-client-0.9.6/sherpa_client/models/suggester_patch.py
+-rw-r--r--   0        0        0     1216 2021-12-02 09:15:42.083660 sherpa-client-0.9.6/sherpa_client/models/suggester_patch_parameters.py
+-rw-r--r--   0        0        0     1498 2021-12-02 09:15:42.111660 sherpa-client-0.9.6/sherpa_client/models/suggestion_facets.py
+-rw-r--r--   0        0        0      655 2021-12-02 09:15:42.079660 sherpa-client-0.9.6/sherpa_client/models/term.py
+-rw-r--r--   0        0        0      837 2021-12-02 09:15:42.095660 sherpa-client-0.9.6/sherpa_client/models/term_hit.py
+-rw-r--r--   0        0        0     1151 2021-12-02 09:15:42.135660 sherpa-client-0.9.6/sherpa_client/models/term_hit_term.py
+-rw-r--r--   0        0        0     1444 2021-12-02 09:15:42.135660 sherpa-client-0.9.6/sherpa_client/models/term_hits.py
+-rw-r--r--   0        0        0     1259 2021-12-02 09:15:42.135660 sherpa-client-0.9.6/sherpa_client/models/term_import.py
+-rw-r--r--   0        0        0     1004 2021-12-02 09:15:42.135660 sherpa-client-0.9.6/sherpa_client/models/term_importer_spec.py
+-rw-r--r--   0        0        0     1229 2021-12-02 09:15:42.151660 sherpa-client-0.9.6/sherpa_client/models/term_importer_spec_parameters.py
+-rw-r--r--   0        0        0      738 2021-12-02 09:15:42.163660 sherpa-client-0.9.6/sherpa_client/models/text_count.py
+-rw-r--r--   0        0        0     2236 2021-12-02 09:15:42.223660 sherpa-client-0.9.6/sherpa_client/models/upload_files_multipart_data.py
+-rw-r--r--   0        0        0     1083 2021-12-02 09:15:42.179660 sherpa-client-0.9.6/sherpa_client/models/uploaded_file.py
+-rw-r--r--   0        0        0      635 2021-12-02 09:15:42.147660 sherpa-client-0.9.6/sherpa_client/models/uploaded_file_info.py
+-rw-r--r--   0        0        0     1280 2021-12-02 09:15:42.211660 sherpa-client-0.9.6/sherpa_client/models/user_permissions_update.py
+-rw-r--r--   0        0        0     1029 2021-12-02 09:15:42.187660 sherpa-client-0.9.6/sherpa_client/models/user_profile_update.py
+-rw-r--r--   0        0        0     2724 2021-12-02 09:15:42.271659 sherpa-client-0.9.6/sherpa_client/models/user_response.py
+-rw-r--r--   0        0        0     2563 2021-12-02 09:15:42.255660 sherpa-client-0.9.6/sherpa_client/models/with_annotator.py
+-rw-r--r--   0        0        0     1206 2021-12-02 09:15:42.207660 sherpa-client-0.9.6/sherpa_client/models/with_annotator_condition.py
+-rw-r--r--   0        0        0     1211 2021-12-02 09:15:42.199660 sherpa-client-0.9.6/sherpa_client/models/with_annotator_parameters.py
+-rw-r--r--   0        0        0     2296 2021-12-02 09:15:42.259660 sherpa-client-0.9.6/sherpa_client/models/with_processor.py
+-rw-r--r--   0        0        0     1206 2021-12-02 09:15:42.223660 sherpa-client-0.9.6/sherpa_client/models/with_processor_condition.py
+-rw-r--r--   0        0        0     1211 2021-12-02 09:15:42.239660 sherpa-client-0.9.6/sherpa_client/models/with_processor_parameters.py
+-rw-r--r--   0        0        0       25 2021-12-02 09:15:30.383702 sherpa-client-0.9.6/sherpa_client/py.typed
+-rw-r--r--   0        0        0     4297 2021-12-02 12:57:22.895589 sherpa-client-0.9.6/sherpa_client/types.py
+-rw-r--r--   0        0        0     5222 2021-12-02 13:42:09.690040 sherpa-client-0.9.6/setup.py
+-rw-r--r--   0        0        0     4139 2021-12-02 13:42:09.690347 sherpa-client-0.9.6/PKG-INFO
```

### Comparing `sherpa-client-0.9.5/LICENSE` & `sherpa-client-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/README.md` & `sherpa-client-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/pyproject.toml` & `sherpa-client-0.9.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sherpa-client"
-version = "0.9.5"
+version = "0.9.6"
 description = "A client library for accessing Sherpa API documentation (Iota release)"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "sherpa_client"},
```

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_binary.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_binary.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_binary_with_plan_ref.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_binary_with_plan_ref.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_corpus_with.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_corpus_with.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_documents_with.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_documents_with.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_documents_with_many.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_documents_with_many.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_binary.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_binary.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_binary_with_plan_ref.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_binary_with_plan_ref.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_documents_with_many.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_documents_with_many.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_documents_with_plan_ref.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_documents_with_plan_ref.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_text_with_many.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_text_with_many.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_format_text_with_plan_ref.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_format_text_with_plan_ref.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_text.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_text.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_text_with.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_text_with.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/annotate_text_with_many.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/annotate_text_with_many.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotate/format_binary.py` & `sherpa-client-0.9.6/sherpa_client/api/annotate/format_binary.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotations/annotation_creators_count.py` & `sherpa-client-0.9.6/sherpa_client/api/annotations/annotation_creators_count.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotations/clear_annotations.py` & `sherpa-client-0.9.6/sherpa_client/api/annotations/clear_annotations.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotations/count_annotations.py` & `sherpa-client-0.9.6/sherpa_client/api/annotations/count_annotations.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotations/create_annotation.py` & `sherpa-client-0.9.6/sherpa_client/api/annotations/create_annotation.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotations/delete_annotation.py` & `sherpa-client-0.9.6/sherpa_client/api/annotations/delete_annotation.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/annotators/get_annotators_by_type.py` & `sherpa-client-0.9.6/sherpa_client/api/annotators/get_annotators_by_type.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/authentication/request_jwt_token.py` & `sherpa-client-0.9.6/sherpa_client/api/authentication/request_jwt_token.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/authentication/user_sign_out.py` & `sherpa-client-0.9.6/sherpa_client/api/authentication/user_sign_out.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/categories/category_creators_count.py` & `sherpa-client-0.9.6/sherpa_client/api/categories/category_creators_count.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/categories/count_categories.py` & `sherpa-client-0.9.6/sherpa_client/api/categories/count_categories.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/categories/create_document_category.py` & `sherpa-client-0.9.6/sherpa_client/api/categories/create_document_category.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/categories/delete_categories.py` & `sherpa-client-0.9.6/sherpa_client/api/categories/delete_categories.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/categories/delete_category.py` & `sherpa-client-0.9.6/sherpa_client/api/categories/delete_category.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/delete_document.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/delete_document.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/export_documents.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/export_documents.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/export_documents_sample.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/export_documents_sample.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/get_document.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/get_document.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/index_document.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/index_document.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/launch_document_import.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/launch_document_import.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/launch_uploaded_document_import.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/launch_uploaded_document_import.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/search_and_delete_documents.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/search_and_delete_documents.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/search_and_export_documents.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/search_and_export_documents.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/search_and_tag_documents.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/search_and_tag_documents.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/search_documents.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/search_documents.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/documents/set_metadata_on_document.py` & `sherpa-client-0.9.6/sherpa_client/api/documents/set_metadata_on_document.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/experiments/cancel_experiment.py` & `sherpa-client-0.9.6/sherpa_client/api/experiments/cancel_experiment.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/experiments/compute_experiment_label_hint.py` & `sherpa-client-0.9.6/sherpa_client/api/experiments/compute_experiment_label_hint.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/experiments/create_experiment.py` & `sherpa-client-0.9.6/sherpa_client/api/experiments/create_experiment.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/experiments/delete_experiment.py` & `sherpa-client-0.9.6/sherpa_client/api/experiments/delete_experiment.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/experiments/delete_experiments.py` & `sherpa-client-0.9.6/sherpa_client/api/experiments/delete_experiments.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/experiments/get_experiment.py` & `sherpa-client-0.9.6/sherpa_client/api/experiments/get_experiment.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/experiments/get_experiments.py` & `sherpa-client-0.9.6/sherpa_client/api/experiments/get_experiments.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/experiments/launch_experiment.py` & `sherpa-client-0.9.6/sherpa_client/api/experiments/launch_experiment.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/experiments/patch_experiment.py` & `sherpa-client-0.9.6/sherpa_client/api/experiments/patch_experiment.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/gazetteers/cancel_synchronize_gazetteer.py` & `sherpa-client-0.9.6/sherpa_client/api/gazetteers/cancel_synchronize_gazetteer.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/gazetteers/compute_gazetteer_label_hint.py` & `sherpa-client-0.9.6/sherpa_client/api/gazetteers/compute_gazetteer_label_hint.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/gazetteers/create_gazetteer.py` & `sherpa-client-0.9.6/sherpa_client/api/gazetteers/create_gazetteer.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/gazetteers/delete_gazetteer.py` & `sherpa-client-0.9.6/sherpa_client/api/gazetteers/delete_gazetteer.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/gazetteers/delete_gazetteers.py` & `sherpa-client-0.9.6/sherpa_client/api/gazetteers/delete_gazetteers.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/gazetteers/export_gazetteer.py` & `sherpa-client-0.9.6/sherpa_client/api/gazetteers/export_gazetteer.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/gazetteers/export_gazetteers.py` & `sherpa-client-0.9.6/sherpa_client/api/gazetteers/export_gazetteers.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/gazetteers/get_gazetteer.py` & `sherpa-client-0.9.6/sherpa_client/api/gazetteers/get_gazetteer.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/gazetteers/get_gazetteers.py` & `sherpa-client-0.9.6/sherpa_client/api/gazetteers/get_gazetteers.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/gazetteers/patch_gazetteer.py` & `sherpa-client-0.9.6/sherpa_client/api/gazetteers/patch_gazetteer.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/gazetteers/synchronize_gazetteer.py` & `sherpa-client-0.9.6/sherpa_client/api/gazetteers/synchronize_gazetteer.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/groups/add_group.py` & `sherpa-client-0.9.6/sherpa_client/api/groups/add_group.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/groups/delete_group.py` & `sherpa-client-0.9.6/sherpa_client/api/groups/delete_group.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/groups/get_group.py` & `sherpa-client-0.9.6/sherpa_client/api/groups/get_group.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/groups/get_groups.py` & `sherpa-client-0.9.6/sherpa_client/api/groups/get_groups.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/groups/patch_group.py` & `sherpa-client-0.9.6/sherpa_client/api/groups/patch_group.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/jobs/cancel_global_job.py` & `sherpa-client-0.9.6/sherpa_client/api/jobs/cancel_global_job.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/jobs/cancel_job.py` & `sherpa-client-0.9.6/sherpa_client/api/jobs/cancel_job.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/jobs/get_all_jobs.py` & `sherpa-client-0.9.6/sherpa_client/api/jobs/get_all_jobs.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/jobs/get_global_job.py` & `sherpa-client-0.9.6/sherpa_client/api/jobs/get_global_job.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/jobs/get_job.py` & `sherpa-client-0.9.6/sherpa_client/api/jobs/get_job.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/jobs/get_jobs.py` & `sherpa-client-0.9.6/sherpa_client/api/jobs/get_jobs.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/jobs/launch_dummy_job.py` & `sherpa-client-0.9.6/sherpa_client/api/jobs/launch_dummy_job.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/jobs/wait_for_job.py` & `sherpa-client-0.9.6/sherpa_client/api/jobs/wait_for_job.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/labels/create_label.py` & `sherpa-client-0.9.6/sherpa_client/api/labels/create_label.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/labels/delete_label_by_name.py` & `sherpa-client-0.9.6/sherpa_client/api/labels/delete_label_by_name.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/labels/get_labels.py` & `sherpa-client-0.9.6/sherpa_client/api/labels/get_labels.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/labels/update_label.py` & `sherpa-client-0.9.6/sherpa_client/api/labels/update_label.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/lexicons/create_lexicon.py` & `sherpa-client-0.9.6/sherpa_client/api/lexicons/create_lexicon.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/lexicons/create_term.py` & `sherpa-client-0.9.6/sherpa_client/api/lexicons/create_term.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/lexicons/delete_lexicon_by_name.py` & `sherpa-client-0.9.6/sherpa_client/api/lexicons/delete_lexicon_by_name.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/lexicons/get_lexicon.py` & `sherpa-client-0.9.6/sherpa_client/api/lexicons/get_lexicon.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/lexicons/get_lexicons.py` & `sherpa-client-0.9.6/sherpa_client/api/lexicons/get_lexicons.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/lexicons/launch_uploaded_terms_import.py` & `sherpa-client-0.9.6/sherpa_client/api/lexicons/launch_uploaded_terms_import.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/lexicons/search_terms.py` & `sherpa-client-0.9.6/sherpa_client/api/lexicons/search_terms.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/lexicons/update_lexicon.py` & `sherpa-client-0.9.6/sherpa_client/api/lexicons/update_lexicon.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/metrics/get_annotation_metrics.py` & `sherpa-client-0.9.6/sherpa_client/api/metrics/get_annotation_metrics.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/metrics/get_categories_metrics.py` & `sherpa-client-0.9.6/sherpa_client/api/metrics/get_categories_metrics.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/metrics/get_corpus_metrics.py` & `sherpa-client-0.9.6/sherpa_client/api/metrics/get_corpus_metrics.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/metrics/get_model_metrics.py` & `sherpa-client-0.9.6/sherpa_client/api/metrics/get_model_metrics.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/models/delete_models.py` & `sherpa-client-0.9.6/sherpa_client/api/models/delete_models.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/plans/compute_plan_label_hint.py` & `sherpa-client-0.9.6/sherpa_client/api/plans/compute_plan_label_hint.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/plans/create_plan.py` & `sherpa-client-0.9.6/sherpa_client/api/plans/create_plan.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/plans/delete_plan.py` & `sherpa-client-0.9.6/sherpa_client/api/plans/delete_plan.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/plans/delete_plans.py` & `sherpa-client-0.9.6/sherpa_client/api/plans/delete_plans.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/plans/get_plan.py` & `sherpa-client-0.9.6/sherpa_client/api/plans/get_plan.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/plans/get_plans.py` & `sherpa-client-0.9.6/sherpa_client/api/plans/get_plans.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/plans/patch_plan.py` & `sherpa-client-0.9.6/sherpa_client/api/plans/patch_plan.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/project_engines/get_project_engine_parameters_schema.py` & `sherpa-client-0.9.6/sherpa_client/api/project_engines/get_project_engine_parameters_schema.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/project_engines/get_project_engines.py` & `sherpa-client-0.9.6/sherpa_client/api/project_engines/get_project_engines.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/project_engines/get_project_services.py` & `sherpa-client-0.9.6/sherpa_client/api/project_engines/get_project_services.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/auto_discover_on_corpus.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/auto_discover_on_corpus.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/compute_train_test_split.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/compute_train_test_split.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/create_project.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/create_project.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/create_project_from_archive.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/create_project_from_archive.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/create_project_from_uploaded_archive.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/create_project_from_uploaded_archive.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/create_tour_project.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/create_tour_project.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/delete_project.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/delete_project.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/delete_tour_project.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/delete_tour_project.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/deploy_project.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/deploy_project.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/export_dataset.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/export_dataset.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/export_models.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/export_models.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/export_project.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/export_project.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/flush_indices.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/flush_indices.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/get_app_state.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/get_app_state.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/get_config.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/get_config.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/get_metadata_definition.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/get_metadata_definition.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/get_project_info.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/get_project_info.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/get_projects.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/get_projects.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/get_properties.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/get_properties.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/import_archive.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/import_archive.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/import_models.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/import_models.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/import_uploaded_archive.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/import_uploaded_archive.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/import_uploaded_models.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/import_uploaded_models.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/launch_project_reindexing.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/launch_project_reindexing.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/launch_project_restoration_from_backup.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/launch_project_restoration_from_backup.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/launch_project_restoration_from_image.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/launch_project_restoration_from_image.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/maybe_create_projects_and_import_models_from_archive.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/maybe_create_projects_and_import_models_from_archive.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/reindex_projects.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/reindex_projects.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/undeploy_project.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/undeploy_project.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/projects/update_config_options.py` & `sherpa-client-0.9.6/sherpa_client/api/projects/update_config_options.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/roles/add_role.py` & `sherpa-client-0.9.6/sherpa_client/api/roles/add_role.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/roles/delete_role.py` & `sherpa-client-0.9.6/sherpa_client/api/roles/delete_role.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/roles/get_permissions.py` & `sherpa-client-0.9.6/sherpa_client/api/roles/get_permissions.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/roles/get_role.py` & `sherpa-client-0.9.6/sherpa_client/api/roles/get_role.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/roles/get_roles.py` & `sherpa-client-0.9.6/sherpa_client/api/roles/get_roles.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/roles/update_role.py` & `sherpa-client-0.9.6/sherpa_client/api/roles/update_role.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/segments/find_similar_segments.py` & `sherpa-client-0.9.6/sherpa_client/api/segments/find_similar_segments.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/segments/get_segment_context.py` & `sherpa-client-0.9.6/sherpa_client/api/segments/get_segment_context.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/segments/search_segments.py` & `sherpa-client-0.9.6/sherpa_client/api/segments/search_segments.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/services/get_engine_parameters_schema.py` & `sherpa-client-0.9.6/sherpa_client/api/services/get_engine_parameters_schema.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/services/get_services.py` & `sherpa-client-0.9.6/sherpa_client/api/services/get_services.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/services/get_services_distinct_values.py` & `sherpa-client-0.9.6/sherpa_client/api/services/get_services_distinct_values.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/shares/change_project_ownership.py` & `sherpa-client-0.9.6/sherpa_client/api/shares/change_project_ownership.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/shares/delete_share_with_group.py` & `sherpa-client-0.9.6/sherpa_client/api/shares/delete_share_with_group.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/shares/delete_share_with_user.py` & `sherpa-client-0.9.6/sherpa_client/api/shares/delete_share_with_user.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/shares/get_group_shares.py` & `sherpa-client-0.9.6/sherpa_client/api/shares/get_group_shares.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/shares/get_user_shares.py` & `sherpa-client-0.9.6/sherpa_client/api/shares/get_user_shares.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/shares/share_with_group.py` & `sherpa-client-0.9.6/sherpa_client/api/shares/share_with_group.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/shares/share_with_user.py` & `sherpa-client-0.9.6/sherpa_client/api/shares/share_with_user.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggesters/compute_suggester_label_hint.py` & `sherpa-client-0.9.6/sherpa_client/api/suggesters/compute_suggester_label_hint.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggesters/create_suggester.py` & `sherpa-client-0.9.6/sherpa_client/api/suggesters/create_suggester.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggesters/delete_suggester.py` & `sherpa-client-0.9.6/sherpa_client/api/suggesters/delete_suggester.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggesters/delete_suggesters.py` & `sherpa-client-0.9.6/sherpa_client/api/suggesters/delete_suggesters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggesters/get_suggester.py` & `sherpa-client-0.9.6/sherpa_client/api/suggesters/get_suggester.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggesters/get_suggesters.py` & `sherpa-client-0.9.6/sherpa_client/api/suggesters/get_suggesters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggesters/patch_suggester.py` & `sherpa-client-0.9.6/sherpa_client/api/suggesters/patch_suggester.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggesters/start_suggester.py` & `sherpa-client-0.9.6/sherpa_client/api/suggesters/start_suggester.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggesters/stop_suggester.py` & `sherpa-client-0.9.6/sherpa_client/api/suggesters/stop_suggester.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggestions/clear_suggestions.py` & `sherpa-client-0.9.6/sherpa_client/api/suggestions/clear_suggestions.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggestions/delete_suggestion.py` & `sherpa-client-0.9.6/sherpa_client/api/suggestions/delete_suggestion.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/suggestions/get_suggestions.py` & `sherpa-client-0.9.6/sherpa_client/api/suggestions/get_suggestions.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/uploads/get_uploaded_file_info.py` & `sherpa-client-0.9.6/sherpa_client/api/uploads/get_uploaded_file_info.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/uploads/upload_files.py` & `sherpa-client-0.9.6/sherpa_client/api/uploads/upload_files.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/users/add_user.py` & `sherpa-client-0.9.6/sherpa_client/api/users/add_user.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/users/delete_user.py` & `sherpa-client-0.9.6/sherpa_client/api/users/delete_user.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/users/get_user.py` & `sherpa-client-0.9.6/sherpa_client/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/users/get_users.py` & `sherpa-client-0.9.6/sherpa_client/api/users/get_users.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/users/update_permissions.py` & `sherpa-client-0.9.6/sherpa_client/api/users/update_permissions.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/api/users/update_profile.py` & `sherpa-client-0.9.6/sherpa_client/api/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/client.py` & `sherpa-client-0.9.6/sherpa_client/client.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/__init__.py` & `sherpa-client-0.9.6/sherpa_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/ack.py` & `sherpa-client-0.9.6/sherpa_client/models/ack.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/aggregation.py` & `sherpa-client-0.9.6/sherpa_client/models/aggregation.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotate_binary_form.py` & `sherpa-client-0.9.6/sherpa_client/models/annotate_binary_form.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotate_binary_with_plan_ref_multipart_data.py` & `sherpa-client-0.9.6/sherpa_client/models/annotate_binary_with_plan_ref_multipart_data.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotate_documents_with_many.py` & `sherpa-client-0.9.6/sherpa_client/models/annotate_documents_with_many.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotate_format_binary_with_plan_ref_multipart_data.py` & `sherpa-client-0.9.6/sherpa_client/models/annotate_format_binary_with_plan_ref_multipart_data.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotate_text_with_many.py` & `sherpa-client-0.9.6/sherpa_client/models/annotate_text_with_many.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotated_doc_annotation.py` & `sherpa-client-0.9.6/sherpa_client/models/annotated_doc_annotation.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotated_doc_annotation_properties.py` & `sherpa-client-0.9.6/sherpa_client/models/annotated_doc_annotation_properties.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotated_doc_category.py` & `sherpa-client-0.9.6/sherpa_client/models/annotated_doc_category.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotated_doc_category_properties.py` & `sherpa-client-0.9.6/sherpa_client/models/annotated_doc_category_properties.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotated_document.py` & `sherpa-client-0.9.6/sherpa_client/models/annotated_document.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotated_document_metadata.py` & `sherpa-client-0.9.6/sherpa_client/models/annotated_document_metadata.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotation.py` & `sherpa-client-0.9.6/sherpa_client/models/annotation.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotation_facets.py` & `sherpa-client-0.9.6/sherpa_client/models/annotation_facets.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotation_id.py` & `sherpa-client-0.9.6/sherpa_client/models/annotation_id.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotation_metrics.py` & `sherpa-client-0.9.6/sherpa_client/models/annotation_metrics.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotation_plan.py` & `sherpa-client-0.9.6/sherpa_client/models/annotation_plan.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotation_term.py` & `sherpa-client-0.9.6/sherpa_client/models/annotation_term.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotation_term_properties.py` & `sherpa-client-0.9.6/sherpa_client/models/annotation_term_properties.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotator.py` & `sherpa-client-0.9.6/sherpa_client/models/annotator.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,48 +10,50 @@
 @attr.s(auto_attribs=True)
 class Annotator:
     """ """
 
     name: str
     label: str
     engine: str
-    favorite: bool
+    favorite: Union[Unset, bool] = UNSET
     is_default: Union[Unset, bool] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         label = self.label
         engine = self.engine
         favorite = self.favorite
         is_default = self.is_default
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
                 "name": name,
                 "label": label,
-                "engine": engine,
-                "favorite": favorite,
+                "engine": engine
             }
         )
+        if favorite is not UNSET:
+            field_dict["favorite"] = favorite
+
         if is_default is not UNSET:
             field_dict["isDefault"] = is_default
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         label = d.pop("label")
 
         engine = d.pop("engine")
 
-        favorite = d.pop("favorite")
+        favorite = d.pop("favorite", UNSET)
 
         is_default = d.pop("isDefault", UNSET)
 
         annotator = cls(
             name=name,
             label=label,
             engine=engine,
```

### Comparing `sherpa-client-0.9.5/sherpa_client/models/annotator_multimap.py` & `sherpa-client-0.9.6/sherpa_client/models/annotator_multimap.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/bearer_token.py` & `sherpa-client-0.9.6/sherpa_client/models/bearer_token.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/bucket.py` & `sherpa-client-0.9.6/sherpa_client/models/bucket.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/categories_facets.py` & `sherpa-client-0.9.6/sherpa_client/models/categories_facets.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/category.py` & `sherpa-client-0.9.6/sherpa_client/models/category.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/category_id.py` & `sherpa-client-0.9.6/sherpa_client/models/category_id.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/category_metrics.py` & `sherpa-client-0.9.6/sherpa_client/models/category_metrics.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/classification_config.py` & `sherpa-client-0.9.6/sherpa_client/models/classification_config.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/classification_options.py` & `sherpa-client-0.9.6/sherpa_client/models/classification_options.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/config_patch_options.py` & `sherpa-client-0.9.6/sherpa_client/models/config_patch_options.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/convert_annotation_plan.py` & `sherpa-client-0.9.6/sherpa_client/models/convert_annotation_plan.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/convert_format_annotation_plan.py` & `sherpa-client-0.9.6/sherpa_client/models/convert_format_annotation_plan.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/converter.py` & `sherpa-client-0.9.6/sherpa_client/models/converter.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/converter_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/converter_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/corpus_metrics.py` & `sherpa-client-0.9.6/sherpa_client/models/corpus_metrics.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/create_lexicon_response_200.py` & `sherpa-client-0.9.6/sherpa_client/models/create_lexicon_response_200.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/create_project_from_archive_multipart_data.py` & `sherpa-client-0.9.6/sherpa_client/models/create_project_from_archive_multipart_data.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/create_term_response_200.py` & `sherpa-client-0.9.6/sherpa_client/models/create_term_response_200.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/created_by_count.py` & `sherpa-client-0.9.6/sherpa_client/models/created_by_count.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/credentials.py` & `sherpa-client-0.9.6/sherpa_client/models/credentials.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/delete_group_result.py` & `sherpa-client-0.9.6/sherpa_client/models/delete_group_result.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/delete_response.py` & `sherpa-client-0.9.6/sherpa_client/models/delete_response.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/doc_annotation.py` & `sherpa-client-0.9.6/sherpa_client/models/doc_annotation.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/doc_category.py` & `sherpa-client-0.9.6/sherpa_client/models/doc_category.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/doc_sentence.py` & `sherpa-client-0.9.6/sherpa_client/models/doc_sentence.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/document.py` & `sherpa-client-0.9.6/sherpa_client/models/document.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/document_facets.py` & `sherpa-client-0.9.6/sherpa_client/models/document_facets.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/document_hit.py` & `sherpa-client-0.9.6/sherpa_client/models/document_hit.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/document_hits.py` & `sherpa-client-0.9.6/sherpa_client/models/document_hits.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/document_metadata.py` & `sherpa-client-0.9.6/sherpa_client/models/document_metadata.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/engine_config.py` & `sherpa-client-0.9.6/sherpa_client/models/engine_config.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/engine_config_import_summary.py` & `sherpa-client-0.9.6/sherpa_client/models/engine_config_import_summary.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/engine_name.py` & `sherpa-client-0.9.6/sherpa_client/models/engine_name.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/experiment.py` & `sherpa-client-0.9.6/sherpa_client/models/experiment.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/experiment_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/experiment_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/experiment_patch.py` & `sherpa-client-0.9.6/sherpa_client/models/experiment_patch.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/experiment_patch_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/experiment_patch_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/format_binary_form.py` & `sherpa-client-0.9.6/sherpa_client/models/format_binary_form.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/format_documents_with_many.py` & `sherpa-client-0.9.6/sherpa_client/models/format_documents_with_many.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/format_text_with_many.py` & `sherpa-client-0.9.6/sherpa_client/models/format_text_with_many.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/formatter.py` & `sherpa-client-0.9.6/sherpa_client/models/formatter.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/formatter_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/formatter_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/gazetteer.py` & `sherpa-client-0.9.6/sherpa_client/models/gazetteer.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/gazetteer_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/gazetteer_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/gazetteer_patch.py` & `sherpa-client-0.9.6/sherpa_client/models/gazetteer_patch.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/gazetteer_patch_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/gazetteer_patch_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/generated_label_hint.py` & `sherpa-client-0.9.6/sherpa_client/models/generated_label_hint.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/get_app_state_response_200.py` & `sherpa-client-0.9.6/sherpa_client/models/get_app_state_response_200.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/get_engine_parameters_schema_response_200.py` & `sherpa-client-0.9.6/sherpa_client/models/get_engine_parameters_schema_response_200.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/get_project_engine_parameters_schema_response_200.py` & `sherpa-client-0.9.6/sherpa_client/models/get_project_engine_parameters_schema_response_200.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/get_suggestions_response_200.py` & `sherpa-client-0.9.6/sherpa_client/models/get_suggestions_response_200.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/group_desc.py` & `sherpa-client-0.9.6/sherpa_client/models/group_desc.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/group_name.py` & `sherpa-client-0.9.6/sherpa_client/models/group_name.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/group_patch.py` & `sherpa-client-0.9.6/sherpa_client/models/group_patch.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/group_share.py` & `sherpa-client-0.9.6/sherpa_client/models/group_share.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/http_service_metadata.py` & `sherpa-client-0.9.6/sherpa_client/models/http_service_metadata.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/http_service_metadata_operations.py` & `sherpa-client-0.9.6/sherpa_client/models/http_service_metadata_operations.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/http_service_record.py` & `sherpa-client-0.9.6/sherpa_client/models/http_service_record.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/import_archive_multipart_data.py` & `sherpa-client-0.9.6/sherpa_client/models/import_archive_multipart_data.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/import_models_multipart_data.py` & `sherpa-client-0.9.6/sherpa_client/models/import_models_multipart_data.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/input_document.py` & `sherpa-client-0.9.6/sherpa_client/models/input_document.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/input_document_metadata.py` & `sherpa-client-0.9.6/sherpa_client/models/input_document_metadata.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/input_label.py` & `sherpa-client-0.9.6/sherpa_client/models/input_label.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/label.py` & `sherpa-client-0.9.6/sherpa_client/models/label.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/label_count.py` & `sherpa-client-0.9.6/sherpa_client/models/label_count.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/label_update.py` & `sherpa-client-0.9.6/sherpa_client/models/label_update.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/launch_document_import_multipart_data.py` & `sherpa-client-0.9.6/sherpa_client/models/launch_document_import_multipart_data.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/launch_project_restoration_from_backup_multipart_data.py` & `sherpa-client-0.9.6/sherpa_client/models/launch_project_restoration_from_backup_multipart_data.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/lexicon.py` & `sherpa-client-0.9.6/sherpa_client/models/lexicon.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/lexicon_update.py` & `sherpa-client-0.9.6/sherpa_client/models/lexicon_update.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/maybe_create_projects_and_import_models_from_archive_multipart_data.py` & `sherpa-client-0.9.6/sherpa_client/models/maybe_create_projects_and_import_models_from_archive_multipart_data.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/metadata_count.py` & `sherpa-client-0.9.6/sherpa_client/models/metadata_count.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/metadata_definition.py` & `sherpa-client-0.9.6/sherpa_client/models/metadata_definition.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/metadata_definition_entry.py` & `sherpa-client-0.9.6/sherpa_client/models/metadata_definition_entry.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/model_metrics.py` & `sherpa-client-0.9.6/sherpa_client/models/model_metrics.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/model_metrics_options.py` & `sherpa-client-0.9.6/sherpa_client/models/model_metrics_options.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/models_metrics.py` & `sherpa-client-0.9.6/sherpa_client/models/models_metrics.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/named_annotation_plan.py` & `sherpa-client-0.9.6/sherpa_client/models/named_annotation_plan.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/new_experiment.py` & `sherpa-client-0.9.6/sherpa_client/models/new_experiment.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/new_experiment_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/new_experiment_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/new_gazetteer.py` & `sherpa-client-0.9.6/sherpa_client/models/new_gazetteer.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/new_gazetteer_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/new_gazetteer_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/new_group_desc.py` & `sherpa-client-0.9.6/sherpa_client/models/new_group_desc.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/new_named_annotation_plan.py` & `sherpa-client-0.9.6/sherpa_client/models/new_named_annotation_plan.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/new_role.py` & `sherpa-client-0.9.6/sherpa_client/models/new_role.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/new_suggester.py` & `sherpa-client-0.9.6/sherpa_client/models/new_suggester.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/new_suggester_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/new_suggester_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/new_user.py` & `sherpa-client-0.9.6/sherpa_client/models/new_user.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/operation_count.py` & `sherpa-client-0.9.6/sherpa_client/models/operation_count.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/partial_label.py` & `sherpa-client-0.9.6/sherpa_client/models/partial_label.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/partial_lexicon.py` & `sherpa-client-0.9.6/sherpa_client/models/partial_lexicon.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/plan_patch.py` & `sherpa-client-0.9.6/sherpa_client/models/plan_patch.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/project_bean.py` & `sherpa-client-0.9.6/sherpa_client/models/project_bean.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/project_config_creation.py` & `sherpa-client-0.9.6/sherpa_client/models/project_config_creation.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/project_config_creation_properties.py` & `sherpa-client-0.9.6/sherpa_client/models/project_config_creation_properties.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/project_property.py` & `sherpa-client-0.9.6/sherpa_client/models/project_property.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/project_status.py` & `sherpa-client-0.9.6/sherpa_client/models/project_status.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/quality_figures.py` & `sherpa-client-0.9.6/sherpa_client/models/quality_figures.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/report.py` & `sherpa-client-0.9.6/sherpa_client/models/report.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/report_classes.py` & `sherpa-client-0.9.6/sherpa_client/models/report_classes.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/role_desc.py` & `sherpa-client-0.9.6/sherpa_client/models/role_desc.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/role_update.py` & `sherpa-client-0.9.6/sherpa_client/models/role_update.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/search_total.py` & `sherpa-client-0.9.6/sherpa_client/models/search_total.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/segment.py` & `sherpa-client-0.9.6/sherpa_client/models/segment.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/segment_context.py` & `sherpa-client-0.9.6/sherpa_client/models/segment_context.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/segment_contexts.py` & `sherpa-client-0.9.6/sherpa_client/models/segment_contexts.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/segment_hit.py` & `sherpa-client-0.9.6/sherpa_client/models/segment_hit.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/segment_hits.py` & `sherpa-client-0.9.6/sherpa_client/models/segment_hits.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/segment_metadata.py` & `sherpa-client-0.9.6/sherpa_client/models/segment_metadata.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/share_mode.py` & `sherpa-client-0.9.6/sherpa_client/models/share_mode.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/sherpa_job_bean.py` & `sherpa-client-0.9.6/sherpa_client/models/sherpa_job_bean.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/sherpa_job_bean_type.py` & `sherpa-client-0.9.6/sherpa_client/models/sherpa_job_bean_type.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/simple_metadata.py` & `sherpa-client-0.9.6/sherpa_client/models/simple_metadata.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/suggester.py` & `sherpa-client-0.9.6/sherpa_client/models/suggester.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/suggester_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/suggester_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/suggester_patch.py` & `sherpa-client-0.9.6/sherpa_client/models/suggester_patch.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/suggester_patch_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/suggester_patch_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/suggestion_facets.py` & `sherpa-client-0.9.6/sherpa_client/models/suggestion_facets.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/term.py` & `sherpa-client-0.9.6/sherpa_client/models/term.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/term_hit.py` & `sherpa-client-0.9.6/sherpa_client/models/term_hit.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/term_hit_term.py` & `sherpa-client-0.9.6/sherpa_client/models/term_hit_term.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/term_hits.py` & `sherpa-client-0.9.6/sherpa_client/models/term_hits.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/term_import.py` & `sherpa-client-0.9.6/sherpa_client/models/term_import.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/term_importer_spec.py` & `sherpa-client-0.9.6/sherpa_client/models/term_importer_spec.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/term_importer_spec_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/term_importer_spec_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/text_count.py` & `sherpa-client-0.9.6/sherpa_client/models/text_count.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/upload_files_multipart_data.py` & `sherpa-client-0.9.6/sherpa_client/models/upload_files_multipart_data.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/uploaded_file.py` & `sherpa-client-0.9.6/sherpa_client/models/uploaded_file.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/uploaded_file_info.py` & `sherpa-client-0.9.6/sherpa_client/models/uploaded_file_info.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/user_permissions_update.py` & `sherpa-client-0.9.6/sherpa_client/models/user_permissions_update.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/user_profile_update.py` & `sherpa-client-0.9.6/sherpa_client/models/user_profile_update.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/user_response.py` & `sherpa-client-0.9.6/sherpa_client/models/user_response.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/with_annotator.py` & `sherpa-client-0.9.6/sherpa_client/models/with_annotator.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/with_annotator_condition.py` & `sherpa-client-0.9.6/sherpa_client/models/with_annotator_condition.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/with_annotator_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/with_annotator_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/with_processor.py` & `sherpa-client-0.9.6/sherpa_client/models/with_processor.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/with_processor_condition.py` & `sherpa-client-0.9.6/sherpa_client/models/with_processor_condition.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/models/with_processor_parameters.py` & `sherpa-client-0.9.6/sherpa_client/models/with_processor_parameters.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/sherpa_client/types.py` & `sherpa-client-0.9.6/sherpa_client/types.py`

 * *Files identical despite different names*

### Comparing `sherpa-client-0.9.5/setup.py` & `sherpa-client-0.9.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 install_requires = \
 ['attrs>=20.1.0,<22.0.0',
  'httpx>=0.15.4,<0.21.0',
  'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'sherpa-client',
-    'version': '0.9.5',
+    'version': '0.9.6',
     'description': 'A client library for accessing Sherpa API documentation (Iota release)',
     'long_description': '# sherpa-client\nA client library for accessing Sherpa API documentation\n\n## Usage\nFirst, create a client:\n\n```python\nfrom sherpa_client import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom sherpa_client import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom sherpa_client.models import MyDataModel\nfrom sherpa_client.api.my_tag import get_my_data_model\nfrom sherpa_client.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom sherpa_client.models import MyDataModel\nfrom sherpa_client.api.my_tag import get_my_data_model\nfrom sherpa_client.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but the async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` by async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `sherpa_client.api.default`\n\n## Building / publishing this Client\nThis project uses [Poetry](https://python-poetry.org/) to manage dependencies  and packaging.  Here are the basics:\n1. Update the metadata in pyproject.toml (e.g. authors, version)\n1. If you\'re using a private repository, configure it with Poetry\n    1. `poetry config repositories.<your-repository-name> <url-to-your-repository>`\n    1. `poetry config http-basic.<your-repository-name> <username> <password>`\n1. Publish the client with `poetry publish --build -r <your-repository-name>` or, if for public PyPI, just `poetry publish --build`\n\nIf you want to install this client into another project without publishing it (e.g. for development) then:\n1. If that project **is using Poetry**, you can simply do `poetry add <path-to-this-client>` from that project\n1. If that project is not using Poetry:\n    1. Build a wheel with `poetry build -f wheel`\n    1. Install that wheel from the other project `pip install <path-to-wheel>`',
     'author': None,
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `sherpa-client-0.9.5/PKG-INFO` & `sherpa-client-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-client
-Version: 0.9.5
+Version: 0.9.6
 Summary: A client library for accessing Sherpa API documentation (Iota release)
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: attrs (>=20.1.0,<22.0.0)
```

