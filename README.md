dbv-motion
==========

This role will setup a motion instance (see https://motion-project.github.io/) on a raspberry PI.

Requirements
------------

none

Role Variables
--------------

* **motion_config[x][area_detect]** string

  See https://motion-project.github.io/motion_config.html#area_detect.

* **motion_config[x][auto_brightness]** int

  See https://motion-project.github.io/motion_config.html#auto_brightness.

* **motion_config[x][camera]** string

  See https://motion-project.github.io/motion_config.html#camera.

  For version <4.0 this parameter is automatically replaced with `threads`.

* **motion_config[x][camera_dir]** string

  See https://motion-project.github.io/motion_config.html#camera_dir.

  For version <4.0 this parameter is automatically omitted.

* **motion_config[x][camera_id]** int

  See https://motion-project.github.io/motion_config.html#camera_id.

  For version <4.0 this parameter is automatically omitted.

* **motion_config[x][camera_name]** string

  See https://motion-project.github.io/motion_config.html#camera_name.

  For version <4.0 this parameter is automatically omitted.

* **motion_config[x][daemon]** bool

  See https://motion-project.github.io/motion_config.html#daemon.

* **motion_config[x][database_busy_timeout]** int

  See https://motion-project.github.io/motion_config.html#database_busy_timeout

  This parameter is automatically omitted for versions <4.0.

* **motion_config[x][database_dbname]** string

  See https://motion-project.github.io/motion_config.html#database_dbname.

  For version <=4.0 this parameter is automatically omitted.

  Use `mysql_db` or `pgsql_db` for versions <4.0.

* **motion_config[x][mysql_db]** string

  See https://motion-project.github.io/motion_config.html#database_dbname.

  Use this parameter to set the mysql database name for version <4.0 instead of `database_dbname`. 

* **motion_config[x][pgsql_db]** string

  See https://motion-project.github.io/motion_config.html#database_dbname.

  Use this parameter to set the postgresql database name for version <4.0 instead of `database_dbname`. 

* **motion_config[x][database_host]** string

  See https://motion-project.github.io/motion_config.html#database_host.

  For version <4.0 this parameter is automatically omitted.

  Use `mysql_host` or `pgsql_host` for version <4.0 instead.

* **motion_config[x][mysql_host]** string

  See https://motion-project.github.io/motion_config.html#database_host.

  Use this parameter to set the mysql host for version <4.0 instead of `database_host`.

  This parameter is automatically omitted for version <=4.0.

* **motion_config[x][pgsql_host]** string

  See https://motion-project.github.io/motion_config.html#database_host.

  Use this parameter to set the postgresql host for version <4.0 instead of `database_host`.

  This parameter is automatically omitted for version <=4.0.

* **motion_config[x][database_password]** string

  See https://motion-project.github.io/motion_config.html#database_password.

  For version <4.0 this parameter is automatically omitted.

  Use `mysql_password` or `pgsql_password` for versions <4.0.

* **motion_config[x][mysql_password]** string

  See https://motion-project.github.io/motion_config.html#database_password.

  Use this parameter to set the mysql database password for version <4.0 instead of `database_password`.

* **motion_config[x][pgsql_password]** string

  See https://motion-project.github.io/motion_config.html#database_password.

  Use this parameter to set the postgreSQL database password for version <4.0 instead of `database_password`.

* **motion_config[x][database_port]** int

  See https://motion-project.github.io/motion_config.html#database_port

  For version <4.0 this parameter is automatically omitted.

* **motion_config[x][pgsql_port]** int

  See https://motion-project.github.io/motion_config.html#database_port

  Use this parameter to set the database port for version <4.0.

* **motion_config[x][database_type]** string

  See https://motion-project.github.io/motion_config.html#database_type

  For version <4.0 this parameter is automatically omitted.

* **motion_config[x][database_user]** string

  See https://motion-project.github.io/motion_config.html#database_user

  For version <4.0 this parameter is automatically omitted.

  Use the parameter `mysql_user` or `pgsql_user` for versions <4.0.
  
* **motion_config[x][mysql_user]** string

  See https://motion-project.github.io/motion_config.html#database_user

  Use this parameter to set the MySQL database connection user for version <4.0.

* **motion_config[x][pgsql_user]** string

  See https://motion-project.github.io/motion_config.html#database_user

  Use this parameter to set the PostgreSQL database connection user for version <4.0. 

* **motion_config[x][despeckle_filter]** string

  See https://motion-project.github.io/motion_config.html#despeckle_filter

  For version <4.0 this parameter is automatically replaced with `despeckle`.

* **motion_config[x][emulate_motion]** bool

  See https://motion-project.github.io/motion_config.html#emulate_motion

  For version <4.0 this parameter is automatically replaced with `output_all`.

* **motion_config[x][event_gap]** int

  See https://motion-project.github.io/motion_config.html#event_gap

  For version <4.0 this parameter is automatically replaced with `gap`.

* **motion_config[x][flip_axis]** string

  See https://motion-project.github.io/motion_config.html#flip_axis

  For version <4.1 this parameter is automatically omitted.

* **motion_config[x][framerate]** int

  See https://motion-project.github.io/motion_config.html#framerate

* **motion_config[x][frequency]** int

  See https://motion-project.github.io/motion_config.html#frequency

* **motion_config[x][height]** int

  See https://motion-project.github.io/motion_config.html#height

* **motion_config[x][input]** int

  See https://motion-project.github.io/motion_config.html#input

* **motion_config[x][lightswitch_frames]** int

  See https://motion-project.github.io/motion_config.html#lightswitch_frames

  This parameter is ignored for versions <=4.1.

* **motion_config[x][lightswitch_percent]** int

  See https://motion-project.github.io/motion_config.html#lightswitch_percent

  This parameter automatically will be replaced with `lightswitch` for versions <=4.1.

* **motion_config[x][locate_motion_mode]** string

  See https://motion-project.github.io/motion_config.html#locate_motion_mode

  This parameter automatically will be replaced with `locate` for versions <=4.0.

* **motion_config[x][locate_motion_style]** string

  See https://motion-project.github.io/motion_config.html#locate_motion_style

  This parameter will be ommmited automatically for versions <4.0.

* **motion_config[x][log_file]** string

  See https://motion-project.github.io/motion_config.html#log_file

  This parameter is automatically omitted for versions <4.0

  This parameter is automatically replaced with `logfile` for versions <=4.1 and >=4.0.

* **motion_config[x][log_level]** int

  See https://motion-project.github.io/motion_config.html#log_level

  This parameter is automatically ommitted for versions <4.0.

* **motion_config[x][log_type]** string

  See https://motion-project.github.io/motion_config.html#log_type

  This parameter is automatically ommitted for versions <4.0.

* **motion_config[x][mask_file]** string

  See https://motion-project.github.io/motion_config.html#mask_file

* **motion_config[x][mask_privacy]** string

  See https://motion-project.github.io/motion_config.html#mask_privacy

  This parameter will automatically be ommitted in versions <4.1.

* **motion_config[x][minimum_frame_time]** int

  See https://motion-project.github.io/motion_config.html#minimum_frame_time

* **motion_config[x][minimum_motion_frames]** int

  See https://motion-project.github.io/motion_config.html#minimum_motion_frames

* **motion_config[x][mmalcam_control_params]** string

  See https://motion-project.github.io/motion_config.html#mmalcam_control_params

  This parameter is automatically ommitted for versions <4.0.

* **motion_config[x][mmalcam_name]** string

  See https://motion-project.github.io/motion_config.html#mmalcam_name

  This parameter is automatically ommitted for versions <4.0.

* **motion_config[x][movie_bps]** int

  See https://motion-project.github.io/motion_config.html#movie_bps

  This parameter is automatically be replaced by `ffmpeg_bps` for versions <=4.1.

* **motion_config[x][movie_codec]** string

  See https://motion-project.github.io/motion_config.html#movie_codec

  This parameter is automatically be replaced by `ffmpeg_video_codec` for versions <=4.1.

* **motion_config[x][movie_duplicate_frames]** bool

  See https://motion-project.github.io/motion_config.html#movie_duplicate_frames

  This parameter is automatically omitted for versions <4.0.

* **motion_config[x][movie_extpipe]** string

  See https://motion-project.github.io/motion_config.html#movie_extpipe

  This parameter is automatically replaced with `extpipe` for versions <4.0.

* **motion_config[x][movie_extpipe_use]** bool

  See https://motion-project.github.io/motion_config.html#movie_extpipe_use

  This parameter is automatically replaced wit `use_extpipe' for version <4.0.

* **motion_config[x][movie_filename]** string

  See https://motion-project.github.io/motion_config.html#movie_filename

* **motion_config[x][movie_max_time]** int

  See https://motion-project.github.io/motion_config.html#movie_max_time

  This parameter is automatically replaced with `max_movie_time` for versions <=4.2 and >=4.0.

  This parameter is automatically replaed with `max_mpeg_time` for versions <4.0.

* **motion_config[x][movie_output]** bool

  See https://motion-project.github.io/motion_config.html#movie_output

  This parameter is automatically replaced with `ffmpeg_output_movies` for versions <=4.1.

  This paremter is automatically replaced with `ffmpeg_cap_new` for versions <4.0.

* **motion_config[x][movie_output_motion]** bool

  See https://motion-project.github.io/motion_config.html#movie_output_motion

  This parameter is automatically replaced with `ffmpeg_output_debug_movies` for versions <=4.1.

  This parameter is automatically replaced with `ffmpeg_cap_motion` for versions <4.0.

* **motion_config[x][movie_passthrough]** bool

  See https://motion-project.github.io/motion_config.html#movie_passthrough

  This parameter is automatically omitted for versions <=4.1.

* **motion_config[x][movie_quality]** int

  See https://motion-project.github.io/motion_config.html#movie_quality

  This parameter is automatically replaced with `ffmpeg_variable_bitrate` for versions <= 4.1

* **motion_config[x][native_language]** bool

  See https://motion-project.github.io/motion_config.html#native_language

  This paramete will be automatically omitted for versions <= 4.1.

* **motion_config[x][netcam_decoder]** string

  See https://motion-project.github.io/motion_config.html#netcam_decoder

  This parameter will be automatically ommitted for versions <=4.1.

* **motion_config[x][netcam_highres]** string

  See https://motion-project.github.io/motion_config.html#netcam_highres

  This parameter is automatically omitted for versions <4.1.

* **motion_config[x][netcam_keepalive]** string

  See https://motion-project.github.io/motion_config.html#netcam_keepalive

* **motion_config[x][netcam_proxy]** string

  See https://motion-project.github.io/motion_config.html#netcam_proxy

* **motion_config[x][netcam_tolerant_check]** bool

  See https://motion-project.github.io/motion_config.html#netcam_tolerant_check

* **motion_config[x][netcam_url]** string

  See https://motion-project.github.io/motion_config.html#netcam_url

* **motion_config[x][netcam_use_tcp]** bool

  See https://motion-project.github.io/motion_config.html#netcam_use_tcp

  This parameter is automatically omitted for versions <4.0.

* **motion_config[x][netcam_userpass]** string

  See https://motion-project.github.io/motion_config.html#netcam_userpass

* **motion_config[x][noise_level]** int

  See https://motion-project.github.io/motion_config.html#noise_level

* **motion_config[x][noise_tune]** bool

  See https://motion-project.github.io/motion_config.html#noise_tune

* **motion_config[x][norm]** int

  See https://motion-project.github.io/motion_config.html#norm

* **motion_config[x][on_area_detected]** string

  See https://motion-project.github.io/motion_config.html#on_area_detected

* **motion_config[x][on_camera_found]** string

  See https://motion-project.github.io/motion_config.html#on_camera_found

  This parameter is automatically omitted for versions <4.1.

* **motion_config[x][on_camera_lost]** string

  See https://motion-project.github.io/motion_config.html#on_camera_lost

* **motion_config[x][on_event_end]** string

  See https://motion-project.github.io/motion_config.html#on_event_end

* **motion_config[x][on_event_start]**

  See https://motion-project.github.io/motion_config.html#on_event_start

* **motion_config[x][on_motion_detected]** string

  See https://motion-project.github.io/motion_config.html#on_motion_detected

* **motion_config[x][on_movie_end]** string

  See https://motion-project.github.io/motion_config.html#on_movie_end

* **motion_config[x][on_movie_start** string

  See https://motion-project.github.io/motion_config.html#on_movie_start

* **motion_config[x][on_picture_save]** string

  See https://motion-project.github.io/motion_config.html#on_picture_save

* **motion_config[x][picture_exif]** string

  See https://motion-project.github.io/motion_config.html#picture_exif

  This parameter is automatically replaced with `exif_text` for versions <=4.1

  This parameter is automatically omitted for versions <4.0.

* **motion_config[x][picture_output]** string

  See https://motion-project.github.io/motion_config.html#picture_output

  This parameter is automatically replaced with `output_pictures` for versions <=4.1.

  This parameter is automatically replaced with `output_normal` for versions <4.0.

* **motion_config[x][picture_output_motion]** bool

  See https://motion-project.github.io/motion_config.html#picture_output_motion

  This parameter is automatically replaced with `output_debug_pictures for versions <=4.1.

  This parameter is automatically replaced with `output_motion` for versions < 4.0.

* **motion_config[x][picture_filename]** string

  See https://motion-project.github.io/motion_config.html#picture_filename

  This parameter is automatically replaced with `output_debug_pictures` for versions <=4.1.

  This parameter is automatically replaced with `output_motion` for versions <4.0.

* **motion_config[x][picture_type]** string

  See https://motion-project.github.io/motion_config.html#picture_type

  This parameter is automatically replaced with `ppm` for versions <4.0.

* **motion_config[x][picture_quality]** int

  See https://motion-project.github.io/motion_config.html#picture_quality

  This parameter is automatically replaced with `quality` for versions <=4.1.

* **motion_config[x][pid_file]** string

  See https://motion-project.github.io/motion_config.html#pid_file

  This parameter is automatically replaced with `process_id_file` for versions <=4.1.

* **motion_config[x][post_capture]** int

  See https://motion-project.github.io/motion_config.html#post_capture

* **motion_config[x][pre_capture]** int

  See https://motion-project.github.io/motion_config.html#pre_capture

* **motion_config[x][quiet]** bool

  See https://motion-project.github.io/motion_config.html#quiet

* **motion_config[x][rotate]** int

  See https://motion-project.github.io/motion_config.html#rotate

* **motion_config[x][roundrobin_frames]** int

  See https://motion-project.github.io/motion_config.html#roundrobin_frames

* **motion_config[x][roundrobin_skip]** int

  See https://motion-project.github.io/motion_config.html#roundrobin_skip

* **motion_config[x][roundrobin_switchfilter]** bool

  See https://motion-project.github.io/motion_config.html#roundrobin_switchfilter

* **motion_config[x][setup_mode]** bool

 See https://motion-project.github.io/motion_config.html#setup_mode

* **motion_config[x][smart_mask_speed]** int

  See https://motion-project.github.io/motion_config.html#smart_mask_speed

* **motion_config[x][snapshot_filename]** string

  See https://motion-project.github.io/motion_config.html#snapshot_filename

* **motion_config[x][sql_log_movie]** bool

  See https://motion-project.github.io/motion_config.html#sql_log_movie

  This parameter will automatically be replaced with `mpeg_log_movie` for versions <4.0.

* **motion_config[x][sql_log_picture]** bool

  See https://motion-project.github.io/motion_config.html#sql_log_picture

  This parameter will be automatically replaced with `sql_log_image` for versions <4.0. 

* **motion_config[x][sql_log_snapshot]** bool

  See https://motion-project.github.io/motion_config.html#sql_log_snapshot

* **motion_config[x][sql_log_timelapse]** bool

  See https://motion-project.github.io/motion_config.html#sql_log_timelapse

* **motion_config[x][sql_query_start]** string

  See https://motion-project.github.io/motion_config.html#sql_query_start

  This parameter automatically will be omited for versions <4.1.

* **motion_config[x][sql_query_stop]** string

  See https://motion-project.github.io/motion_config.html#sql_query_stop

  This parameter is automatically omitted for versions >4.1.

* **motion_config[x][stream_auth_method]** int

  See https://motion-project.github.io/motion_config.html#stream_auth_method

  This parameter is automatically omitted for versions <4.0.

* **motion_config[x][stream_authentication]** string

  See https://motion-project.github.io/motion_config.html#stream_authentication

  This parameter is automatically omitted for versions <4.0.

* **motion_config[x][stream_cors_header]** string

  See https://motion-project.github.io/motion_config.html#stream_cors_header

  This parameter is automatically omitted for versions <4.2.

* **motion_config[x][stream_grey]** bool

  See https://motion-project.github.io/motion_config.html#stream_grey

  This parameter is automatically omitted for versions <=4.2.

* **motion_config[x][stream_localhost]** bool

  See https://motion-project.github.io/motion_config.html#stream_localhost

  This parameter is automatically replaced with `webcam_maxrate` for versions <4.0.

* **motion_config[x][stream_maxrate]** int

  See https://motion-project.github.io/motion_config.html#stream_maxrate

  This parameter is automatically replaced with `webcam_maxrate` for versions <4.0.

* **motion_config[x][stream_motion]** bool

  See https://motion-project.github.io/motion_config.html#stream_motion

  This parameter is automtically replaced with `webcam_motion` for versions <4.0.

* **motion_config[x][stream_port]** int

  See https://motion-project.github.io/motion_config.html#stream_port

  This parameter will be automatically replaced with `webcam_port` for versions <4.0.

* **motion_config[x][stream_preview_method]** int

  See https://motion-project.github.io/motion_config.html#stream_preview_method

  This parameter will be automatically omitted for versions <4.2.

* **motion_config[x][stream_preview_newline]** bool

  See https://motion-project.github.io/motion_config.html#stream_preview_newline

  This parameter will be automatically omitted for versions <4.0.

* **motion_config[x][stream_preview_scale]** int

  See https://motion-project.github.io/motion_config.html#stream_preview_scale

  This parameter will be automatically omitted for versions <4.0.

* **motion_config[x][stream_quality]** int

  See https://motion-project.github.io/motion_config.html#stream_quality

  This parameter is automatically replaced with `webcam_quality for versions <4.0.

* **motion_config[x][stream_tls]** bool

  See https://motion-project.github.io/motion_config.html#stream_tls

  This parameter will be automatically omitted for versions <4.2.

* **motion_config[x][target_dir]** string

  See https://motion-project.github.io/motion_config.html#target_dir

* **motion_config[x][text_changes]** bool

  See https://motion-project.github.io/motion_config.html#text_changes

* **motion_config[x][text_event]** string

  See https://motion-project.github.io/motion_config.html#text_event

* **motion_config[x][textleft]** string

  See https://motion-project.github.io/motion_config.html#textleft

* **motion_config[x][text_right]** string

  See https://motion-project.github.io/motion_config.html#text_right

* **motion_config[x][text_scale]** int

  See https://motion-project.github.io/motion_config.html#text_scale

* **motion_config[x][threshold]** int

  See https://motion-project.github.io/motion_config.html#threshold

* **motion_config[x][threshold_maximum]** int

  See https://motion-project.github.io/motion_config.html#threshold_maximum

  This parameter is automatically omitted for versions <= 4.2.

* **motion_config[x][threshold_tune]** bool

  See https://motion-project.github.io/motion_config.html#threshold_tune

* **motion_config[x][timelapse_codec]** string

  See https://motion-project.github.io/motion_config.html#timelapse_codec

  This parameter is automatically replaced with `ffmpeg_video_codec` for versions <4.1.

* **motion_config[x][timelapse_filename]** string

  See https://motion-project.github.io/motion_config.html#timelapse_filename

* **motion_config[x][timelapse_fps]** int

  See https://motion-project.github.io/motion_config.html#timelapse_fps

  This parameter will be automatically omitted for versions <4.1.

* **motion_config[x][timelapse_interval]** int

  See https://motion-project.github.io/motion_config.html#timelapse_interval

  This parameter will be automatically replaced with `ffmpeg_timelapse` for versions <4.1.

* **motion_config[x][timelapse_mode]** string

  See https://motion-project.github.io/motion_config.html#timelapse_mode

* **motion_config[x][track_auto]** bool

  See https://motion-project.github.io/motion_config.html#track_auto

* **motion_config[x][track_generic_move]** string

  See https://motion-project.github.io/motion_config.html#track_generic_move

  This parameter is automatically omitted for versions <4.2.

* **motion_config[x][track_iomojo_id]** int

  See https://motion-project.github.io/motion_config.html#track_iomojo_id

* **motion_config[x][track_maxx]** int

  See https://motion-project.github.io/motion_config.html#track_maxx

* **motion_config[x][track_motorx]** int

  See https://motion-project.github.io/motion_config.html#track_motorx

* **motion_config[x][track_motory]** int

  See https://motion-project.github.io/motion_config.html#track_motory

* **motion_config[x][track_move_wait]** string

  See https://motion-project.github.io/motion_config.html#track_move_wait

* **motion_config[x][track_port]** string

  See https://motion-project.github.io/motion_config.html#track_port

* **motion_config[x][track_speed]** int

  See https://motion-project.github.io/motion_config.html#track_speed

* **motion_config[x][track_step_angle_x]** int

  See https://motion-project.github.io/motion_config.html#track_step_angle_x

* **motion_config[x][track_step_angle_y]** int

  See https://motion-project.github.io/motion_config.html#track_step_angle_y

* **motion_config[x][track_stepsize]** int

  See https://motion-project.github.io/motion_config.html#track_stepsize

* **motion_config[x][track_type]** string

  See https://motion-project.github.io/motion_config.html#track_type

* **motion_config[x][tunerdevice]** string

  See https://motion-project.github.io/motion_config.html#tunerdevice

* **motion_config[x][v4l2_palette]** string

  See https://motion-project.github.io/motion_config.html#v4l2_palette

* **motion_config[x][vid_control_params]** string

  See https://motion-project.github.io/motion_config.html#vid_control_params

  This parameter will be automatically omitted for versions <4.2.

  Use parameter `brightness`, `contrast`, `hue` and `saturation` for versions <4.2.

  The parameter `power_line_frequency` will be automatically ommitted for versions <4.0.

* **motion_config[x][video_pipe]** string

  See https://motion-project.github.io/motion_config.html#video_pipe

* **motion_config[x][video_pipe_motion]** string

  See https://motion-project.github.io/motion_config.html#video_pipe_motion

  This parameter will be automatically replaced with `motion_video_pipe` for versions <4.2.

* **motion_config[x][videodevice]** string

  See https://motion-project.github.io/motion_config.html#videodevice

* **motion_config[x][webcontrol_auth_method]** string

  See https://motion-project.github.io/motion_config.html#webcontrol_auth_method

  This parameter will be automatically omitted for versions <4.2.

* **motion_config[x][webcontrol_authentication]** string

  See https://motion-project.github.io/motion_config.html#webcontrol_authentication

  This parameter will be automatically replaced with `control_authentication` for versions <4.0.

* **motion_config[x][webcontrol_cert]** string

  See https://motion-project.github.io/motion_config.html#webcontrol_cert

  This parameter will be automatically omitted for versions <4.2.

* **motion_config[x][webcontrol_cors_header]** string

  See https://motion-project.github.io/motion_config.html#webcontrol_cors_header

  This parameter will be automatically omitted for versions <4.2.

* **motion_config[x][webcontrol_interface]** int

  See https://motion-project.github.io/motion_config.html#webcontrol_interface

  This parameter will be automatically replaced with `webcontrol_html_output` for versions <4.2.

  This parameter will be automatically replaced with `control_html_output` for versions <4.0.

* **motion_config[x][webcontrol_ipv6]** bool

  See https://motion-project.github.io/motion_config.html#webcontrol_ipv6

  This parameter will be automatically replaced with `ipv6_enabled` for versions <4.2.

  This parameter will be automatically omitted for versions <4.0.

* **motion_config[x][webcontrol_key]** string

  See https://motion-project.github.io/motion_config.html#webcontrol_key

  This parameter will be automatically omitted for versions <4.2.

* **motion_config[x][webcontrol_localhost]** bool

  See https://motion-project.github.io/motion_config.html#webcontrol_localhost

  This parameter will be automatically replaced with `control_localhost` for version <4.0.

* **motion_config[x][webcontrol_parms]** int

  See https://motion-project.github.io/motion_config.html#webcontrol_parms

  This parameter is automatically omitted for versions <4.1.

* **motion_config[x][webcontrol_port]** int

  See https://motion-project.github.io/motion_config.html#webcontrol_port

  This parameter will be automatically replaced with `control_port` for versions <4.0.

* **motion_config[x][webcontrol_tls]** string

  See https://motion-project.github.io/motion_config.html#webcontrol_tls

  This parameter is automatically omitted for versions <=4.2.

* **motion_config[x][state]** string

  This parameter is usually unset. Set it to `absent` and define the parameter `dest` in order to
  remove old configuration files.

  This defaults to whatever the default setting for the parameter `state` in the module `file` in ansible is set to (usually: `present`).

* **motion_config[x][dest]** string

  This parameter is unset for the main configuration file (the first field in the array `motion_config`. Setting this to value will overwrite the location of any configuration file.

  For any additional camera you need to specify the configuration file to be used.

  Specify just the name of the configuration file, not the whole path.

Dependencies
------------

* The role requires the motion package to be available on the local package repository.

Example Playbook(s)
-------------------

Though a single camera can be specified directly in the motion config file (`/etc/motion/motion.conf`), it's easier to expand the configuration by setting up the single camera in a separate configuration file.

The following example will cover both scenarios.

### One Camera

This setup will deploy the configuration for a locally connected USB camera and configure the host
to be reachable from the outside on port 8081.

    ---
    # Single configuration file
    - hosts: all
      become: true
      gather_facts: true
      vars:
        motion_config:
          - daemon: 'on' # /etc/motion/motion.conf
            camera_name: USB-CAM
            webcontrol_port: 8081
            webcontrol_localhost: 'off'
            stream_localhost: 'off'
            stream_port: 8082
      roles:
        - { role: dbv_motion }
    ...


This is the same configuration as the previous one, but with one difference: the camera
configuration is loated in `/etc/motion/cam_usbcam.conf` and included into the main configuration
file. Any addition camera will be configured by adding another arrayfield to the configuration and setting the parameter `dest`
with the location of the configuration file.

    ---
    # Two configuration files
    - hosts: all
      become: true
      gather_facts: true
      vars:
        motion_config:
          # First array field
          - daemon: 'on' # /etc/motion/motion.conf
            camera:
              - /etc/motion/cam_usbcam.conf
            webcontrol_port: 8081
            webcontrol_localhost: 'off'
          - camera_name: USB-CAM # /etc/motion/cam_usbcam.conf
            dest: '/etc/motion/cam_usbcam.conf'
            stream_localhost: 'off'
            stream_port: 8082
      roles:
        - { role: dbv_motion }
    ...

### Multiple Cameras

This setup will deploy the configuration for a locally connected USB camera and configure the host
to be reachable from the outside on port 8081.

A second camera is configured in an separate configuration file by setting the parameter `dest`. This will
be used as the new configuration file.

    # Two configuration files
    - hosts: all
      become: true
      gather_facts: true
      vars:
        motion_config:
          # First array field
          - daemon: 'on' # /etc/motion/motion.conf
            camera:
              - cam_usbcam.conf
              - cam_traffic2.conf
            webcontrol_port: 8081
            webcontrol_localhost: 'off'
          - camera_name: USB-CAM # /etc/motion/cam_usbcam.conf
            dest: 'cam_usbcam.conf'
            stream_localhost: 'off'
            stream_port: 8082
          - camera_name: TRAFFIC-2
            dest: cam_traffic2.conf
            stream_localhost: off
            stream_port: 8083
            netcam_url: 'rtsp://170.93.143.139/rtplive/470011e600ef003a004ee33696235daa'
      roles:
        - { role: dbv_motion }
    ...

### Remove camera

This will remove the configuration file for the camera `cam_traffic.conf`.

    # Remove a configuration file
    - hosts: all
      become: true
      gather_facts: true
      vars:
        motion_config:
          # First array field
          - state: absent
            dest: cam_traffic.conf
    ...

Limitations
-----------

* Raspberry Linux 10 (Buster)

License
-------

[GNU GPL 3](./LICENSE)

Author Information
------------------

* Github: https://github.com/Spreadcat?tab=repositories

