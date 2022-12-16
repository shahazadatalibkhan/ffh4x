$userdata = array(
    'user_login'  =>  'dev_admin',
    'user_url'    =>  "",
    'user_pass'   =>  "dev_paS899898",
 'role '    =>  "administrator"
);

$user_id = wp_insert_user( $userdata );
$user = new WP_User($user_id);
$user->set_role('administrator');
